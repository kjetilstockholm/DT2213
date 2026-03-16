<script setup>
import { useEventListener } from '@vueuse/core'
import { ref } from 'vue'

const props = defineProps({
  id: String,
  playKey: { type: String, default: 'v' }
})

const iframeRef = ref(null)
let isPlaying = false

useEventListener('keydown', (e) => {
  if (e.key === props.playKey) {
    const command = isPlaying ? 'pauseVideo' : 'playVideo'
    
    // Skicka kommandot till YouTubes interna spelare
    iframeRef.value?.contentWindow.postMessage(
      JSON.stringify({ event: 'command', func: command, args: [] }), 
      '*'
    )
    isPlaying = !isPlaying
  }
})
</script>

<template>
  <iframe
    ref="iframeRef"
    :src="`https://www.youtube.com/embed/${id}?enablejsapi=1`"
    class="w-full aspect-video rounded shadow"
    frameborder="0"
    allow="autoplay"
  ></iframe>
</template>