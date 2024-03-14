<script setup>

import IconArrowLeft from "@/components/icons/page_fourth/IconArrowLeft.vue";
</script>

<template>
    <div class="header">
        <div class="IconArrowLeft arrow">
            <IconArrowLeft/>
        </div>
        <p class="pageName" ref="pageName">Nasz zespół</p>
        <div class="IconArrowRight arrow">
            <IconArrowLeft/>
        </div>
    </div>
</template>

<style scoped>
.header {
    position: relative;
    margin: 30px 128px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}

@media (min-width: 630px) {
    .pageName {
        min-width: 300px;
    }
}

@media (max-width: 630px) {
    .header {
        margin: 30px 16px;
    }

    .arrow {
        display: none;
    }
}

.pageName {
    flex: 1;
    font-size: 48px;
    font-weight: 700;
    text-align: center;
    margin: 32px;
    text-shadow: 0 -10px 100px #FFF;
}

.IconArrowLeft {
    flex-grow: 1;
    overflow: hidden;
}

.IconArrowRight {
    flex-grow: 1;
    overflow: hidden;
    transform: matrix(-1, 0, 0, 1, 0, 0);
}
</style>