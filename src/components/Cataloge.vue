<script setup>
import { Icon } from '@iconify/vue';
import TopCategories from './elements/TopCategories.vue';
import Product from './elements/Product.vue';

const nex = [{
  title:"D By Diesel",category:"Perfume",price:1600, img:"https://media.theperfumeshop.com/medias/sys_master/prd-images/hbb/hbb/8920356978718/prd-front-1286313_420x420/prd-front-1286313-420x420.jpg"
},
{
  title:"Lovely You",category:"Eau de Parfum Gift Set",price:1600, img:"https://media.theperfumeshop.com/medias/sys_master/prd-images/h71/h55/8909586956318/prd-front-1289603_420x420/prd-front-1289603-420x420.jpg"
},
{
  title:"Princess",category:"Eau de Toilette Spray",price:1600, img:"https://media.theperfumeshop.com/medias/zoom-front-1053768-420x420?context=bWFzdGVyfHByZC1pbWFnZXN8MTI3MDg2fGltYWdlL2pwZWd8aDlkL2hiZC84ODI2NDI2MTYzMjMwL3pvb20tZnJvbnQtMTA1Mzc2OF80MjB4NDIwfDE2MjJmNWJhMjg1ODlhYmNlZGU5NzI3NmRiODM4ZTRiYzg4YTQwZmY1ZTA4M2E2NWM2MWE1YmM2OGNhYjIyYzE"
},
{
  title:"D By Diesel",category:"Perfume",price:1600, img:"https://media.theperfumeshop.com/medias/sys_master/prd-images/hbb/hbb/8920356978718/prd-front-1286313_420x420/prd-front-1286313-420x420.jpg"
}]

</script>
<template>
    <div class="w-full flex flex-col gap-10">
   <div class="w-full rounded overflow-hidden">
    <!-- ADS -->
    <img src="https://marketplace.canva.com/EAFKuV12aEA/1/0/1600w/canva-orange-and-yellow-vibrant-shoe-sale-mobile-banner-yuUYhVOB8b0.jpg"/>
   </div>    
 <div class="w-full flex gap-10">
  <div class="w-full flex  flex-col gap-10">
    <div class="flex justify-start">
      <ul class="flex items-center gap-10">
        <li class="hover:text-[#ec4132]  ">Best</li>
        <li>Most seller</li>
        <li>New</li>
        <li>hear</li>
      </ul>
    </div>

    <div class="flex w-full flex-wrap justify-around gap-3">
      <Product v-for="(items, indes) in nex" :category="items.category" :title="items.title" :img="items.img" :price="items.price"/> 
    </div>

  </div>
  <!-- <div class=" flex flex-1">
    <img src="https://marketplace.canva.com/EAFnvat1cmY/1/0/427w/canva-lfI2Yu-UXcY.jpg" alt=""/>
  </div> -->

</div>
<TopCategories/>
    </div>
</template>
