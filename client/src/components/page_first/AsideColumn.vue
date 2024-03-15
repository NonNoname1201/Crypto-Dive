<script setup>
import IconBigLogo from '../icons/page_first/IconBigLogo.vue';
import {defineComponent} from 'vue';

const components = {
    IconBigLogo,
};
</script>

<template>
    <section class="aside-first-page">
        <IconBigLogo/>
        <img src="../icons/page_first/GreenLight.png" alt="GreenLight" class="green-light">
    </section>
</template>

<style scoped>
.aside-first-page {
    height: 100vh;
    display: flex;
    align-items: center;


    svg {
        height: 50vh;
        width: auto;
        margin-right: 7vw;
    }

    img {
        position: absolute;
        right: 0;
        z-index: -1;
    }

    position: absolute;
    right: 0;
    z-index: 0;
}
</style>