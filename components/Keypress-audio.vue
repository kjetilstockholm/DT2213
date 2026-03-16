<script setup>
import { useEventListener } from '@vueuse/core'
import { ref, watch } from 'vue'

const props = defineProps({
  src: { type: String, required: true },
  playKey: { type: String, default: 'm' },
  // Vi skickar med den aktuella sidans nummer
  page: { type: Number }
})

const audioRef = ref(null)

useEventListener('keydown', (e) => {
  // KOLL: Vi kollar om tangenten är rätt OCH om vi är på rätt slide
  // Slidev injicerar automatiskt $nav i templaten, men här i script använder vi props
  if (e.key === props.playKey) {
    if (audioRef.value) {
      audioRef.value.currentTime = 0
      audioRef.value.play()
    }
  }
})
</script>

<template>
  <audio 
    v-if="$nav.currentPage === $page"
    ref="audioRef" 
    :src="src" 
    preload="auto" 
    class="hidden" 
  />
</template>