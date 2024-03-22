<script setup>
import {onMounted} from 'vue';
import PageFirst from '@/components/PageFirst.vue';
import PageSecond from '@/components/PageSecond.vue';
import PageThird from '@/components/PageThird.vue';
import PageFourth from "@/components/PageFourth.vue";

import Footer from "@/components/Footer.vue";

onMounted(() => {
    document.title = "Crypto Dive";
});
</script>

<template>

    <PageFirst/>
    <PageSecond/>
    <PageThird/>
    <PageFourth/>
    <Footer/>
</template>

<style scoped>

</style>
