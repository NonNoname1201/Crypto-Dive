<script setup>
import {onMounted} from 'vue';
import PageFirst from '@/components/PageFirst.vue';
import PageSecond from '@/components/PageSecond.vue';
import PageThird from '@/components/PageThird.vue';
import PageFourth from "@/components/PageFourth.vue";
import Foreground from "@/components/Foreground.vue";

onMounted(() => {
    document.title = "Crypto Dive";
});
</script>

<template>
    <Foreground/>
    <PageFirst/>
    <PageSecond/>
    <PageThird/>
    <PageFourth/>
</template>

<style scoped>

</style>
