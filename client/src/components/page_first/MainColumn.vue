<script setup>
import Logo from '../icons/page_first/IconLogo.vue';
import Star from '../icons/page_first/IconStar.vue';


import { defineComponent, ref } from 'vue';

const navigateToLink = () => {
  window.location.href = 'https://discord.gg/ZXbAnv8SVC';
};

defineComponent({
  methods: {
    navigateToLink,
  },
});

const components = {
    Logo,
    Star,
};
</script>

<template>
    <section class="first-page">
        <Logo/>
        <div class="text-box">
            <h1 class="Intro-text">CRYPTO DIVE - To <br><span class="green-text">pierwszy</span> projrekt <br>edukacji <span
                class="blue-text">Krypto<br></span> w Polsce!
                <Star class="star"/>
            </h1>
            <div class="gradient-line"></div>
        </div>
        <button class="entry-button" @click="navigateToLink">
            Rozpocząć
        </button>
    </section>
</template>

<style scoped>

.entry-button {
    width: 170px;
    height: 40px;
    border: 4px solid white;
    background-color: #000000;
    border-radius: 10px;
    transition: border 1s ease-in;
    text-decoration: none;
    color: white;
    font-size: 20px;
    font-weight: 700;
    cursor: pointer;
}

.entry-button:hover {
    background: linear-gradient(black, black) padding-box, linear-gradient(270deg, #7000FF 0%, #0075FF 49%, #33FF00 100%) border-box;
    border-radius: 10px;
    border: 4px solid transparent;
}


.first-page {
    padding: 7vh 0 15vh 7vw;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    gap: 3vh;
    h1 {
        font-size: clamp(30px, 8vh, 50px);
        font-weight: 800;
        word-wrap: break-word;
        background: transparent;
    }

    .star {
        height: clamp(20px, 4vh, 30px);
        background: transparent;
    }

    text-align: left;

    .green-text {
        color: #51FF82;
        background: transparent;
    }

    .blue-text {
        color: #2395FF;
        background: transparent;
    }

    .gradient-line {
        margin-top: 3vh;
        width: 25vw;
        height: 15px;
        background: linear-gradient(270deg, #7000FF 0%, #0075FF 49%, #33FF00 100%);
        border-radius: 12px;
    }

    background: transparent;
    z-index: 1;
}
</style>