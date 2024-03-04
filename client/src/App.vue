<script setup>
import FirstPage from '@/components/PageFirst.vue';
import SecondPage from '@/components/PageSecond.vue';
import ThirdPage from '@/components/PageThird.vue';
import { defineComponent } from 'vue';

const components = {
  FirstPage,
  SecondPage,
  ThirdPage,
};
</script>

<template>
  <FirstPage />
  <ThirdPage />
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
