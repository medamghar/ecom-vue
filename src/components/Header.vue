<script setup>
import { Icon } from "@iconify/vue";
import DropdownSelect from './elements/DropdownSelect.vue'
import Logo from '../assets/logo.svg'



</script>



<template>
  <div class="flex justify-between w-full items-center">
    <div>
      <h1>JmlaShop.ma</h1>
    </div>
    <div class="border-slate-200 border w-[36rem]">
      <div class=" h-12 flex items-center ">
        <div class="grow px-2">
          <input placeholder="hi there" class="h-12 w-full text-12" />
        </div>
        <div class="border-l w-40 h-12 flex justify-center items-center">
        <DropdownSelect/>
        </div>
        <div class="bg-[#189ffa] h-12 w-12 justify-center items-center flex"><Icon color="white" icon="iconoir:search" width="32" height="32" /></div>

      </div>
    </div>
    <div class="flex gap-12">
      <div class="flex items-center gap-1">
        <Icon icon="ph:user" width="36" height="36" />
        <div class="flex flex-col"> 
         <span class="text-xs text-[#8c8b8b]">Sign In</span>
         <span class="text-sm font-medium ">Account</span>
        </div>
      </div>
      <div>
        <Icon icon="iconoir:heart" width="36" height="36" />

      </div>
      <div class="flex items-center gap-1">
        <Icon icon="tdesign:cart" width="36" height="36" />
        <div class="flex flex-col"> 
         <span class="text-xs text-[#8c8b8b]">Total</span>
         <span class="text-sm font-medium ">$10.00</span>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
