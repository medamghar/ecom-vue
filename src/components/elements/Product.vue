<script setup>
import { Icon } from "@iconify/vue";
defineProps({
  title: String,
  category: String,
  img: String,
  price: Number,
});
</script>
<template>
  <div
    class=" relative flex flex-col w-[17.6rem] h-84 overflow-hidden product bg-[#fbfbfb] rounded transition ease-in-out delay-150 hover:-translate-y-1 hover:scale-110 duration-100"
  >
  <div class="w-36 h-8 z-10 bg-[#f87171]
 rotate-[130deg] absolute top-5 left-[-50px] 	">
   
</div>
<span class="absolute z-10 top-5 font-bold text-white rotate-[-50deg] left-[-8px]">PROMO!</span>
    <div class="relative m-2 rounded overflow-hidden">
      <img loading="lazy" :src="img" class="w-72 h-56" />
      <div
        class="absolute w-6 h-6 rounded-full bg-white top-2 right-2 flex justify-center items-center"
      >
        <Icon icon="mdi:heart-outline" />
      </div>
      
    </div>
    <div class="flex flex-col gap-2 p-2">
      <div class="w-full flex justify-between items-center">
        <span class="text-xs font-bold text-[#19a0fc]">{{ category }}</span>
        <span
          class="text-xs px-4 text-white bg-red-400 font-medium rounded-full"
          >-35%</span
        >
      </div>
      <div class="flex justify-between">
        <h1 class="font-bold text-md">{{ title }}</h1>
        <span class="text-[#ec4132] font-bold">{{ price }}DH</span>
      </div>
      <div class="w-full relative">
        <button
          class="px-4 w-full py-1 rounded text-white bg-[#189ffa] font-medium text-sm"
        >
          Add to cart
        </button>
      </div>
    </div>
  </div>
</template>
