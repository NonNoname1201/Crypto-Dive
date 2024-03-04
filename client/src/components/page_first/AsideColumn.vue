<script setup>
import Planet from '../icons/page_first/IconPlanet.vue';
import { defineComponent } from 'vue';

const components = {
  Planet,
};
</script>

<template>
  <section class="aside-first-page">
    <Planet />
  </section>
</template>

<style scoped>
.aside-first-page {
  height: 100vh;

  svg {
    height: 100vh;
  }

  margin-left: -500px;
}
</style>