<template>
  <div class="slidev-layout default w-full h-full flex flex-col">
    <div class="w-full mb-4 text-left">
      <slot />
    </div>

    <div class="grid grid-cols-2 gap-8 items-start flex-grow">
      
      <div class="flex flex-col text-left">
        <slot name="left" />
      </div>

      <div class="flex flex-col text-left">
        <slot name="right" />
      </div>
      
    </div>
  </div>
  
  
  <div class="grid grid-cols-[6fr_4fr] flex-grow relative">
  <div class="relative"> <slot name="left" />
  </div>
  <div class="relative overflow-hidden"> <slot name="right" />
  </div>
</div>
  
</template>