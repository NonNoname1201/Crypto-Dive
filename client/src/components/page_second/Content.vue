<script setup>
import { ref, onMounted, onUnmounted } from 'vue';
import PageThin from "@/components/page_second/PageThin.vue";
import PageMedium from "@/components/page_second/PageMedium.vue";
import PageWide from "@/components/page_second/PageWide.vue";

const currentPage = ref(null);
let divHeight = ref(0);

const updateCurrentPage = () => {
  const width = window.innerWidth;
  divHeight.value = document.querySelector('.content').clientHeight;
  const height = divHeight.value;
  //this div

  if (width/height <= 670.0/700) {
    currentPage.value = PageThin;
  } else if (width/height <= 1024.0/700) {
    currentPage.value = PageMedium;
  } else {
    currentPage.value = PageWide;
  }
};

onMounted(() => {
  divHeight.value = document.querySelector('.content').clientHeight;
  window.addEventListener('resize', updateCurrentPage);
  updateCurrentPage();
});

onUnmounted(() => {
  window.removeEventListener('resize', updateCurrentPage);
});
</script>

<template>
  <div class="content">
    <component :is="currentPage" />
  </div>
</template>

<style scoped>

</style>