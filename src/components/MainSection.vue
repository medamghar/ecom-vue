<script setup>
import MainSlide from './MainSlide.vue';
import SideBar from './SideBar.vue';
import { Icon } from '@iconify/vue';
import { data } from '../assets/lib/data';
</script>
<template>
  <div class="flex flex-col gap-10">
  <div class="flex gap-10">
    <SideBar/>
    <MainSlide/>
    
  </div>
 
  
    <div class="flex justify-between items-center">
      <div v-for="(item, index) in data" :key="index" class="flex gap-5 items-center">
        <div class="bg-[#fff1f0] w-20 h-20 rounded-full flex justify-center items-center">
          <Icon :icon="item.icon" color="#eb4732" width="36" height="36" />
        </div>
        <div class="flex flex-col gap-1">
          <h1 class="font-medium">{{ item.title }}</h1>
          <span class="text-[#a8a8a8]  text-xs">{{ item.description }}</span>
        </div>
      </div>
    </div>


</div>

</template>

