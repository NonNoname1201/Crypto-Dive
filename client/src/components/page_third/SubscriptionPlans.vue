<script setup>
import PlanOneMonth from "@/components/page_third/PlanOneMonth.vue";
import PlanSixMonths from "@/components/page_third/PlanSixMonths.vue";
import PlanUnlimited from "@/components/page_third/PlanUnlimited.vue";
import {defineComponent} from 'vue';

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
        <PlanOneMonth/>
        <PlanSixMonths/>
        <PlanUnlimited/>
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
        color: #fff;
        font-size: 30px;
        font-weight: 900;
    }

    h4 {
        color: #989898;
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
    padding-left: 3vw;
    padding-right: 3vw;
    display: flex;
    flex-direction: row;
    gap: 3vw;
    justify-content: space-around;
    align-items: flex-start;
    flex-wrap: wrap;
    min-height: 80vh;
}

.description-item:nth-child(1) {
    border: 10px solid #434343;
    border-radius: 25px;
    box-shadow: none;
    transition: transform 0.3s, box-shadow 0.8s 0.3s;
}

.description-item:nth-child(1):hover {
    transform: scale(1.01);
    box-shadow: 0 0 40px 15px #FFFFFF80;
}

.description-item:nth-child(2) {
    background: linear-gradient(black, black) padding-box, linear-gradient(45deg, rgb(219, 0, 255), rgb(36, 0, 255)) border-box;
    border-radius: 25px;
    border: 10px solid transparent;
    box-shadow: none;
    transition: transform 0.3s, box-shadow 0.8s 0.3s;
}

.description-item:nth-child(2):hover {
    transform: scale(1.01);
    box-shadow:
        -15px -15px 40px rgba(94, 0, 255, 0.4),
        15px -15px 40px rgba(28, 0, 255, 0.4),
        15px 15px 40px rgba(120, 0, 255, 0.4),
        -15px 15px 40px rgba(219, 0, 255, 0.4);
}


.description-item:nth-child(3) {
    background: linear-gradient(black, black) padding-box, linear-gradient(45deg, rgb(255, 255, 255), rgb(255, 229, 0)) border-box;
    border-radius: 25px;
    border: 10px solid transparent;
    box-shadow: none;
    transition: transform 0.3s, box-shadow 0.8s 0.3s;
}

.description-item:nth-child(3):hover {
    transform: scale(1.01);
    box-shadow:
        -15px -15px 40px rgba(255, 255, 130, 0.4),
        15px -15px 40px rgba(255, 225, 20, 0.4),
        15px 15px 40px rgba(255, 255, 130, 0.4),
        -15px 15px 40px rgba(255, 255, 255, 0.4);
}


.description-item {
    flex: 1;

    color: #fff;
    min-width: 360px;
    max-width: 400px;
    height: 500px;
}
</style>