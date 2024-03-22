<script setup>
import GreyStar from "@/components/icons/page_third/IconGreyStar.vue";
import IconConfirm from "@/components/icons/page_third/IconConfirm.vue";

const components = {
    GreyStar,
};
</script>

<template>
    <div class="description-item">
        <div class="title">
            Dive Club<br>1 miesiąc
            <GreyStar/>
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
            <p class="price">199 ZŁ<span class="small-letters">/mies</span></p>
            <button class="button-style">
                <IconConfirm/>
                <a>Kupić</a>
            </button>
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
    border-top: 6px solid #434343;
    border-bottom: 6px solid #434343;
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
        font-family: Inter, sans-serif;
        font-size: 25px;
        font-weight: 800;
        .small-letters {
            font-size: 17px;
        }
    }

    .button-style {
        font-size: 25px;
        font-weight: 700;
        padding: 5px 20px 5px 10px;
        background: black;
        border: 5px solid #434343;
        border-radius: 20px;

        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
        gap: 10px;
        cursor: pointer;
        transition: transform 0.3s;
    }

    .button-style:hover {
        transform: scale(1.01);
    }
}
</style>