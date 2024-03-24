<script setup>
import {defineProps} from 'vue';

const props = defineProps({
    name: String,
    position: String,
    photoUrl: String,
    instagramUrl: String,
    telegramUrl: String
});

import IconInstagram from "@/components/icons/page_fourth/IconInstagram.vue";
import IconTelegram from "@/components/icons/page_fourth/IconTelegram.vue";
</script>

<template>
    <div class="card">
        <div class="photoContainer">
            <div class="photo" :style="{ backgroundImage: `url(${photoUrl})` }"></div>
        </div>
        <div class="description">
            <p class="name">{{ name }}</p>
            <p class="position">{{ position }}</p>
        </div>
        <div class="contact">
            <a :href="instagramUrl" target="_blank" class="icon">
                <IconInstagram/>
            </a>
            <a :href="telegramUrl" target="_blank" class="icon">
                <IconTelegram/>
            </a>
        </div>
    </div>
</template>

<style scoped>
.card {
    margin: 0 16px 32px 16px;
    transition: transform 0.3s;
}

.card:hover {
    transform: scale(1.05);
    transition: transform 0.3s, box-shadow 0.8s 0.3s;;
    .photoContainer {
        transition: box-shadow 0.8s 0.3s;
        box-shadow: 0 0 40px 10px rgba(81, 255, 129, 0.5);
    }
}

.photoContainer {
    height: 372px;
    width: 290px;
    border-radius: 15px;
    transition: box-shadow 0.8s 0.3s;
    box-shadow: 0 0 30px 10px rgba(81, 255, 129, 0.3);
}

.photo {
    height: 100%;
    width: 100%;
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

.icon {
    margin: 0 12px 0 0;
}
</style>