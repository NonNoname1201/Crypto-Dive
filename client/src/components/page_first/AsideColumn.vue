<script setup>
  import Planet from '../icons/page_first/IconPlanet.vue';
  export default {
    components: {
      Planet,
    },
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

  Planet {
    height: 100vh;
  }

  margin-left: -500px;
}
</style>