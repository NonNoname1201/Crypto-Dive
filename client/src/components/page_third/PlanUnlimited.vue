<script setup>
import GoldenStar from "@/components/icons/page_third/IconGoldenStar.vue";
import IconConfirm from "@/components/icons/page_third/IconConfirm.vue";
</script>

<template>
    <div class="description-item">
        <div class="title">
            Dive Club Premium<br>&infin;
            <GoldenStar/>
        </div>
        <div class="description">
            <ul>
                <li>Wszystkie korzyści wynikające z subskrypcji Dive Club VIP</li>
                <li>Dożywotna subskrypcja</li>
                <li>Ekskluzywne spotkania</li>
                <li>Bonus <span class="bold-number">70</span>% za każdego poleconego</li>
            </ul>
        </div>
        <div class="price-section">
            <p class="price">2999 ZŁ</p>
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
        padding: 5px 20px 5px 10px;
        background: linear-gradient(black, black) padding-box, linear-gradient(45deg, rgb(255, 255, 255), rgb(255, 229, 0)) border-box;
        border-radius: 20px;
        border: 5px solid transparent;

        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
        gap: 10px;
        cursor: pointer;
        transition: transform 0.3s;
    }

    .button-style:hover {
        transform: scale(1.02);
    }
}
</style>