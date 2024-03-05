<script setup>
import PageFirst from '@/components/PageFirst.vue';
import PageSecond from '@/components/PageSecond.vue';
import PageThird from '@/components/PageThird.vue';
import { defineComponent } from 'vue';

const components = {
  FirstPage,
  SecondPage,
  ThirdPage,
};
</script>

<script>
export default {
  data() {
    return {
      title: 'Crypto Dive'
    }
  },
  mounted() {
    document.title = this.title;
  }
}
</script>

<template>
  <header>
  </header>

  <main>
    <PageFirst />
    <PageSecond/>
    <PageThird />
  </main>
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
