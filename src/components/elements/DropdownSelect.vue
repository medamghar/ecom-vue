<script setup >
import { Icon } from '@iconify/vue';
import { ref } from 'vue';
const isOpen = ref(false)
const data = ref("Select categories")

</script>
<template>
    <div class="w-full relative">
     <div @click="isOpen=!isOpen"  class="h-12 font-normal flex justify-between items-center p-2">
        <span>{{ data }}</span>
        <Icon icon="ep:arrow-down" :class="{ 'rotate-180': isOpen }" />
    
     </div>
     <ul  v-if="isOpen" class="absolute z-10 buttom-0 left-0  bg-white  w-full shadow-2xl rounded">
        <li @click="data='nice'"  value="nice1" class="h-12 px-2 hover:bg-[#189ffa] text-base hover:text-white  flex items-center">nice</li>
        <li value="nice2" class="h-12 px-2 hover:bg-[#189ffa] text-base hover:text-white  flex items-center ">nice</li>
        <li value="nice3" class="h-12 px-2 hover:bg-[#189ffa] text-base hover:text-white  flex items-center">nice</li>

     </ul>
    </div>
</template>