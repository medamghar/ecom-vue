<script setup>
import { Icon } from '@iconify/vue';
import { ref } from 'vue';
const isOpen = ref(false)
const isHovered = ref(false)

</script>

<template>
    <div class="w-[20%]  flex flex-col" >
    <div class="w-full h-12 bg-red-600 flex gap-4 items-center px-4  text-white ">
        <Icon   icon="ic:round-menu" width="30" height="30"/> 
        <span class="text-sm">Browser all categories</span>
        

    </div>
    <div class="flex flex-col bg-[#f9f9f9] w-full items-center divide-y ">
      <div  class="w-full h-12 flex justify-between items-center px-4 hover:bg-red-200" @mouseover="isOpen=true" @mouseleave="isOpen=false" >
        

          <span>
        Electronics
       </span>
       <Icon :class="{ 'rotate-180 transition ease-in-out ': isOpen }"  icon="iconamoon:arrow-right-2" width="32" height="32"/>
        

    
      </div>
      <div class="w-full h-12 flex justify-between items-center px-4" >
       <span>
        Electronics
       </span>
       <Icon icon="iconamoon:arrow-right-2" width="32" height="32"/>

      </div>
      <div class="w-full h-12 flex justify-between items-center px-4" >
       <span>
        Electronics
       </span>
       <Icon icon="iconamoon:arrow-right-2" width="32" height="32"/>

      </div>
      <div class="w-full h-12 flex justify-between items-center px-4" >
       <span>
        Electronics 
       </span>
       <Icon icon="iconamoon:arrow-right-2" width="32" height="32"/>

      </div>
      <div class="w-full h-12 flex justify-between items-center px-4" >
       <span>
        Electronics
       </span>
       <Icon icon="iconamoon:arrow-right-2" width="32" height="32"/>

      </div>
    </div>
    </div>
</template>