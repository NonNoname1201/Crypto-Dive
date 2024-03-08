<script setup>

</script>

<template>
    <div class="header">
        <p class="pageName" ref="pageName">Nasz ekosystem</p>
    </div>
</template>

<style scoped>
.header {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 60px;
}

.pageName {
    font-size: 50px;
    font-weight: 700;
    line-height: 61px;
    padding-bottom: 14px;
    text-align: center;

    background: linear-gradient(black, black) padding-box, linear-gradient(270deg, #BD00FF 0%, #0047FF 53%, #31FA0B 100%) border-box;
    border-bottom: 6px solid transparent;
}

</style>