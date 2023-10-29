<script setup>
import { Icon } from '@iconify/vue';
import TopCategories from './elements/TopCategories.vue';

const nex = [1,2,3,4,5,6,7,8,]

</script>
<template>
    <div class="w-full flex flex-col gap-10">
       
 <div class="w-full flex gap-10">
  <div class="w-[80%] flex  flex-col gap-10">
    <div class="flex justify-end">
      <ul class="flex items-center gap-5">
        <li class="hover:text-[#ec4132]  ">Best</li>
        <li>Most seller</li>
        <li>New</li>
        <li>hear</li>
      </ul>
    </div>

    <div class="flex w-full flex-wrap gap-3">
     
        <div v-for="(items, indes) in nex" class="flex flex-col w-56 h-80 overflow-hidden product bg-[#fbfbfb] rounded transition ease-in-out delay-150  hover:-translate-y-1 hover:scale-110 duration-100">
        <div>
            <img src="https://cdn.pixabay.com/photo/2018/02/01/19/21/easter-3123834_1280.jpg" class="w-56 h-56"/>
        </div>
        <div class="flex flex-col gap-2 p-2">
            <div class="w-full flex justify-between">
                <span class="text-xs font-bold text-[#19a0fc]">Chocoalte</span>
                <Icon icon="gridicons:add-outline" color="#a8a8a8" width="20" height="20" />
            </div>
            <div class="flex justify-between ">
                <h1 class="font-medium text-md">Colored chocoalte egges</h1>
                <span class="text-[#ec4132] font-bold">126DH</span>
            </div>
            
        
        </div>
      </div>
    </div>
  </div>
  <div class=" flex flex-1">
    <img src="https://marketplace.canva.com/EAFnvat1cmY/1/0/427w/canva-lfI2Yu-UXcY.jpg" alt=""/>
  </div>

</div>
<TopCategories/>
    </div>
</template>
