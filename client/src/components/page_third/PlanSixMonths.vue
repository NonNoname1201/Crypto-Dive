<script setup>
import BlueStar from "@/components/icons/page_third/IconBlueStar.vue";

const components = {
    BlueStar,
};
</script>

<template>
    <div class="description-item">
        <div class="title">
            Dive Club VIP<br>6 miesiące
            <BlueStar/>
        </div>
        <div class="description">
            <ul>
                <li>Wczesny dostęp do wszystkich aktywności</li>
                <li>Bonus <span class="bold-number">60</span>% za każdego poleconego</li>
                <li>Dostęp do prywatwych maretyli</li>
                <li>Spersonalizowane wsparcie</li>
                <li>Wyłączna rola</li>
                <li>Wczesny dostęp do wszystich nowych produktów</li>
            </ul>
        </div>
        <div class="price-section">
            <p class="price">999 ZŁ</p>
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
    background: transparent;

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
    background: transparent;
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
        background: linear-gradient(black, black) padding-box, linear-gradient(45deg, rgb(219, 0, 255), rgb(36, 0, 255)) border-box;
        border-radius: 10px;
        border: 5px solid transparent;
    }

}
</style>