<script setup>

import IconInstagram from "@/components/icons/page_fourth/IconInstagram.vue";
import IconTelegram from "@/components/icons/page_fourth/IconTelegram.vue";
</script>

<template>
    <div class="card">
        <div class="photoContainer">
            <div class="photo"></div>
        </div>
        <div class="description">
            <p class="name">Maksim Slysh</p>
            <p class="position">Content manager</p>
        </div>
        <div class="contact">
            <a href="" target="_blank" class="icon"><IconInstagram/></a>
            <a href="" target="_blank" class="icon"><IconTelegram/></a>
        </div>
    </div>
</template>

<style scoped>
.card {
}

.photoContainer {
    height: 372px;
    width: 290px;
    border-radius: 20%;
    box-shadow: 0 0 110px 10px rgba(112, 1, 255, 0.3);
}

.photo {
    height: 100%;
    width: 100%;
    background-image: url("../../assets/photoMaksim.png");
    background-size: cover;
    background-position: center;
}

.description {
}

.name {
    font-size: 32px;
    font-weight: 700;
    padding: 12px 0;
}

.position {
    font-size: 20px;
    font-weight: 500;
    padding-bottom: 10px;
}

.contact {
}

.icon{
    margin: 0 12px 0 0;
}
</style>