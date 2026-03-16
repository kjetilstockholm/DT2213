<template>
  <div class="slidev-layout h-full grid grid-cols-[7fr_3fr] gap-8">
    
    <div class="pt-[50px]">
      <slot /> </div>
    
    <div class="flex flex-col items-center justify-center">
      <slot name="right" /> </div>

  </div>
</template>