<script setup>
import {ref, onMounted, onUnmounted} from 'vue';

let y = ref( window.innerHeight);
let lastScrollPosition = window.innerHeight;

const updatePosition = () => {
    let currentScrollPosition = window.scrollY;
    if (currentScrollPosition > lastScrollPosition) {
        y.value = currentScrollPosition;
    }
    lastScrollPosition = currentScrollPosition;
};

onMounted(() => {
    window.addEventListener('scroll', updatePosition);
});

onUnmounted(() => {
    window.removeEventListener('scroll', updatePosition);
});
</script>

<template>
    <div class="foreground" :style="{ transform: `translate3d(0, ${y}px, 0)` }"></div>
</template>

<style scoped>
.foreground {
    width: 100%;
    height: 200vh;
    position: absolute;
    background: linear-gradient(0deg, rgba(0, 0, 0, 1), rgba(0, 0, 0, 1), rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0));
    z-index: 10;
    transition: transform 0.5s ease-out;
}
</style>