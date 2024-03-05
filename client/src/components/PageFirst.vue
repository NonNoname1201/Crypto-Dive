<script setup>
import MainColumn from "@/components/page_first/MainColumn.vue";
import AsideColumn from "@/components/page_first/AsideColumn.vue";
import { defineComponent } from 'vue';

const components = {
  MainColumn,
  AsideColumn,
};
</script>

<template>
  <div class="Page-first page">
    <MainColumn />
    <AsideColumn />
  </div>
</template>

<style scoped>
  .Page-first {
    display: flex;
    text-align: center;
  }
</style>