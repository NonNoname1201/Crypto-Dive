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
  margin-right: -200px;
  position: absolute;
  right: 0;
  z-index: 0;
}
</style>