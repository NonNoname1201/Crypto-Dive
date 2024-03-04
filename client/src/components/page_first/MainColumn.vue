<script setup>
import Logo from '../icons/page_first/IconLogo.vue';
import Star from '../icons/page_first/IconStar.vue';
import { defineComponent } from 'vue';

const components = {
  Logo,
  Star,
};
</script>

<template>
  <section class="first-page">
    <Logo />
    <h1 class="Intro-text">CRYPTO Dive - To <br><span class="green-text">pierwszy</span> projrekt <br>edukacji <span class="blue-text">kryptowalutowej<br></span> w Polsce!  <Star class="star"/></h1>
    <div class="gradient-line"></div>
    <button class="entry-button"><a href="https://discord.gg/ZXbAnv8SVC">Rozpocząć</a></button>
  </section>
</template>

<style scoped>
.entry-button {
  width: 285px;
  height: 79px;
  border: 5px solid white;
  background-color: #000000;
  border-radius: 15px;
  a {
    text-decoration: none;
    color: white;
    font-size: 40px;
    font-weight: 700;
  }
}
.first-page {
  h1 {
    font-size: 50px;
    font-weight: 800;
    word-wrap: break-word;
  }

  .star {
    height: 30px;
  }

  text-align: left;

  .green-text {
    color: #51FF82;
  }

  .blue-text {
    color: #2395FF;
  }

  .gradient-line {
    width: 30vw;
    height: 15px;
    background: linear-gradient(270deg, #7000FF 0%, #0075FF 49%, #33FF00 100%);
    border-radius: 12px;
  }
}
</style>