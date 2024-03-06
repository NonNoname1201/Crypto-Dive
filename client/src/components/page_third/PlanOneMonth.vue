<script setup>
import GreyStar from "@/components/icons/page_third/IconGreyStar.vue";
import { defineComponent } from 'vue';

const components = {
  GreyStar,
};
</script>

<template>
  <div class="description-item">
    <div class="title">
      Dive Club<br>1 miesiąc
      <GreyStar />
    </div>
    <div class="description">
      <ul>
        <li>Wczesny dostęp do wszystkich aktywności</li>
        <li>Bonus <span class="bold-number">50</span>% za każdego poleconego</li>
        <li>Dostęp do prywatwych maretyli</li>
        <li>Spersonalizowane wsparcie</li>
        <li>Wyłączna rola</li>
      </ul>
    </div>
    <div class="price-section">
      <p class="price">199 ZŁ</p>
      <button class="button-style"><a>Kupić</a></button>
    </div>
  </div>
</template>

<style scoped>
.title {
  padding: 30px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  font-size: clamp(10px, 4vw, 20px);
  font-weight: 900;
  border: none;
  border-radius: 10px;
  height: 20%;
}

.description {
  border-top: 3px solid #434343;
  border-bottom: 3px solid #434343;
  font-weight: 500;
  font-size: 17px;
  height: 55%;
  padding: 25px 28px;
  ul {
    list-style-image: url('@/components/icons/page_third/plan_list_icon.svg');
    li {
      padding-bottom: 4px;
    }
  }
}

.price-section {
  padding: 25px;
  height: 25%;
  border-radius: 10px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  .price {
    font-size: 25px;
    font-weight: 800;
  }

  .button-style {
    font-size: 25px;
    font-weight: 700;
    padding: 5px 30px;
    border: 5px solid #434343;
    border-radius: 10px;
  }
}
</style>