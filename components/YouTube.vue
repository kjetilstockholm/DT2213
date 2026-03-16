<template>
  <div class="my-4 flex justify-center">
    <iframe
      :width="width"
      :height="height"
      :src="`https://www.youtube.com/embed/${id}?start=${start}&autoplay=${autoplay ? 1 : 0}&mute=${muted ? 1 : 0}&rel=0`"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
      class="rounded-lg shadow-lg"
    ></iframe>
  </div>
</template>

<script setup>
defineProps({
  id: String,
  width: { default: '100%' },
  height: { default: '400' },
  start: { default: 0 },
  autoplay: { type: Boolean, default: false },
  muted: { type: Boolean, default: false } // Autoplay kräver ofta mute=true för att garanteras
})
</script>