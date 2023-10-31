<script setup>
import Cataloge from './components/Cataloge.vue';
import Header from './components/Header.vue'
import Layout from './components/Layout.vue'
import MainSection from './components/MainSection.vue';
import Footer from './components/Footer.vue';
</script>

<template>
<Layout #layout>
    <div class="flex flex-col gap-10">
        <Header/>
<MainSection/>
<Cataloge/>
<Footer/>
    </div>

</Layout>

</template>

<style scoped>
</style>
