<template>

  <div class="fixed inset-0 pointer-events-none z-50">
    
    <img 
      v-if="$nav.currentPage !== 1"
      src="/KTH_logo_RGB_bla.svg" 
      class="absolute bottom-2 left-2 h-8" 
    />

    <img 
      v-if="$nav.currentPage === 1"
      src="/KTH_logo_RGB_vit.svg" 
      class="absolute top-[7%] left-1/2 -translate-x-1/2 w-45" 
    />
  </div>

  <div 
    v-if="$slidev.nav.currentPage !== 1 && $slidev.nav.currentPage !== $slidev.nav.total"
    class="absolute bottom-3 left-12 text-[10px] flex gap-2"
    style="color: var(--slidev-theme-primary);"
  >
    <span>{{ $slidev.configs.course_code }}</span>
    <span class="opacity-50">|</span>
    <span>{{ $slidev.configs.lecture_title }}</span>
    <span class="opacity-50">|</span>
    <span>{{ $slidev.configs.lecturer }}</span>
    <span class="opacity-50">|</span>
    <span>{{ $slidev.nav.currentPage }} / {{ $slidev.nav.total }}</span>
  </div>
</template>