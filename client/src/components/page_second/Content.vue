<script setup>

import IconNews from "@/components/icons/page_second/IconNews.vue";
import IconMoney from "@/components/icons/page_second/IconMoney.vue";
import IconStudent from "@/components/icons/page_second/IconStudent.vue";
import IconMember from "@/components/icons/page_second/IconMember.vue";
import IconStarCenter from "@/components/icons/page_second/IconStarCenter.vue";
</script>

<template>
    <div class="Content">
        <div class="block">
            <p>Na naszym kanale informacyjnym jako pierwszy dowiesz się
                o wszystkich najważniejszych wiadomościach w przestrzeni
                kryptowalutowej.</p>
            <div class="placeholder"></div>
            <div class="iconBorder">
                <IconNews class="iconContent"/>
            </div>
        </div>

        <div class="block">
            <p>Na kanale kryptоaktywności codziennie zobaczysz wszystkie
                szczegółowe instrukcje dotyczące zarabiania pierwszych
                pieniędzy w kryptowalutach.</p>
            <div class="placeholder"></div>
            <div class="iconBorder">
                <IconMoney class="iconContent"/>
            </div>
        </div>

        <div class="block">
            <p>W sekcji szkoleniowej znajdziesz naszą książkę napisaną
                przez założyciela firmy oraz podstawowe koncepcje
                i działania w kryptowalutach
                w przejrzystej formie.</p>
            <div class="placeholder"></div>
            <div class="iconBorder">
                <IconStudent class="iconContent"/>
            </div>
        </div>

        <div class="block">
            <p>
                Dive Club to miejsce, gdzie nauczysz się pomnażać swoje
                zyski z kryptowalut. Dołącz
                do prywatnej społeczności z ludźmi o podobnych
                pasjach i odblokuj bonusowe nagrody. </p>
            <div class="placeholder"></div>
            <div class="iconBorder">
                <IconMember class="iconContent"/>
            </div>
        </div>
        <IconStarCenter class="iconCenter"/>
    </div>
</template>

<style scoped>
.Content {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    padding: 20px;
    margin: 0 100px;
}

.block {
    flex: 1;
    max-width: 560px;
    min-width: 400px;
    min-height: 16rem;
    width: 40%;

    position: relative;
    margin: 23px;
    padding: 20px 120px 20px 20px;

    background: rgba(0, 0, 0, 0.8);
    border: 4px solid #51ff81;
    border-radius: 30px;
    overflow: hidden;
}

p {
    font-size: 25px;
    text-align: left;
}

.iconBorder {
    position: absolute;
    bottom: -25px;
    right: -25px;

    padding: 35px 40px 40px 35px;
    border: 4px solid #51ff81;
    border-radius: 100%;
}

.iconContent {
    width: 65px;
    height: 65px;
    filter: drop-shadow(0 0 40px #FFF);
}

@media (max-width: 1131.5px) {
    .iconCenter {
        display: none;
    }
}

@media (min-width: 1577px) {
    .iconCenter{
        display: none;
    }
}

.iconCenter {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}
</style>