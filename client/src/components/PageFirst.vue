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
  <div class="Page-first">
    <MainColumn />
    <AsideColumn />
  </div>
</template>

<style scoped>
  .Page-first {
    background: black;
    background-size: auto 100vh;
    width: 100%;
    min-height: 100vh;
    color: white;
    display: flex;
    text-align: center;
  }
</style>