<script setup>
import PlanOneMonth from "@/components/page_third/PlanOneMonth.vue";
import PlanSixMonths from "@/components/page_third/PlanSixMonths.vue";
import PlanUnlimited from "@/components/page_third/PlanUnlimited.vue";
import { defineComponent } from 'vue';

const components = {
  PlanOneMonth,
  PlanSixMonths,
  PlanUnlimited,
};
</script>

<template>
  <section class="wrapper">
    <section class="header">
      <h1>Kup subskypcję w <span class="gradient-text">najlepszej cenie</span></h1>
      <h4>Cena subskrypcji rośnie z każdą większa aktualizacją</h4>
    </section>
    <section class="description-container">
      <PlanOneMonth />
      <PlanSixMonths />
      <PlanUnlimited />
    </section>
  </section>
</template>

<style scoped>
.wrapper {
background: black;
}
.header {
  height: 20vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

h1 {
  color : #fff;
  font-size: 30px;
  font-weight: 900;
}

h4 {
  color : #989898;
  font-size: 15px;
  font-weight: 700;
}

.gradient-text {
  background: linear-gradient(to right, rgb(219, 0, 255), rgb(85, 54, 255));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.description-container {
  height: 80vh;
  display: flex;
}

.description-item {
  flex: 1;
  margin: 0 3vw 3vw 3vw;
  border: 1px solid #333;
  color: #fff;
}
</style>