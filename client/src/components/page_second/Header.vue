<script setup>
import IconStarFilled from "@/components/icons/page_second/IconStarHeader.vue";
</script>

<template>
    <div class="header">
        <IconStarFilled class="IconStarFilled"/>
        <p class="pageName" ref="pageName">Nasz ekosystem</p>
        <IconStarFilled class="IconStarFilled"/>
    </div>
</template>

<style scoped>
.header {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;

    padding-top: 60px;
}

.IconStarFilled {
    margin: 0 32px;
    width: 38px;
    height: 38px;

    filter: drop-shadow(0 0 30px #FFF);

}

.pageName {
    font-size: 40px;
    font-weight: 700;
    text-align: center;
    background: transparent;

    padding: 16px 34px;
    border: 4px solid #51ff81;
    border-radius: 19px;

    text-shadow: 0 -10px 100px #FFF;
}
</style>