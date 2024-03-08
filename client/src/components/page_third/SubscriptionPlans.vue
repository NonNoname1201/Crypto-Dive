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
  <section class="header">
    <h1>Kup subskypcję w <span class="gradient-text">najlepszej cenie</span></h1>
    <h4>Cena subskrypcji rośnie z każdą większa aktualizacją</h4>
  </section>
  <section class="description-container">
    <PlanOneMonth />
    <PlanSixMonths />
    <PlanUnlimited />
  </section>
</template>

<style scoped>
.header {
  height: 20vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
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
}

.description-container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}

.description-item:nth-child(1) {
  border: 6px solid #434343;
  border-radius: 10px;
}
.description-item:nth-child(2) {
  background: linear-gradient(black, black) padding-box, linear-gradient(45deg, rgb(219, 0, 255), rgb(36, 0, 255)) border-box;
  border-radius: 10px;
  border: 6px solid transparent;
}


.description-item:nth-child(3) {
  background: linear-gradient(black, black) padding-box, linear-gradient(45deg, rgb(255, 255, 255), rgb(255, 229, 0)) border-box;
  border-radius: 10px;
  border: 6px solid transparent;
}


.description-item {
  flex: 1;
  margin: 0 3vw 3vw 3vw;
  color: #fff;
  min-width: 400px;
  max-width: 450px;
  height: 500px;
}
</style>