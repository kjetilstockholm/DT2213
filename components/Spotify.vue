<template>
  <iframe
    class="rounded-xl my-4"
    :src="`https://open.spotify.com/embed/${type}/${id}?utm_source=generator&autoplay=${autoplay ? 1 : 0}`"
    width="100%"
    :height="height"
    frameBorder="0"
    allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
  ></iframe>
</template>

<script setup>
defineProps({
  id: String,
  type: { default: 'track' },
  height: { default: '80' },
  autoplay: { type: Boolean, default: false }
})
</script>