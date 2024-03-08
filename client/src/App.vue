<script setup>
import PageFirst from '@/components/PageFirst.vue';
import PageSecond from '@/components/PageSecond.vue';
import PageThird from '@/components/PageThird.vue';

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
    <PageSecond />
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
</style>
