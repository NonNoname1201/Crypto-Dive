<script setup>
import {onMounted} from 'vue';
import PageFirst from '@/components/PageFirst.vue';
import PageSecond from '@/components/PageSecond.vue';
import PageThird from '@/components/PageThird.vue';
import PageFourth from "@/components/PageFourth.vue";

onMounted(() => {
    document.title = "Crypto Dive";
});
</script>

<template>
    <main>
        <PageFirst/>
        <PageSecond/>
        <PageThird/>
        <PageFourth/>
    </main>
</template>

<style scoped>
main {
    background-image: url("./assets/tile.png");
    background-repeat: repeat;
}
</style>
