<script setup>

import Header from "@/components/page_fourth/Header.vue";
import MemberCard from "@/components/page_fourth/MemberCard.vue";
</script>

<template>
    <div class="Page-fourth page">
        <div class="header">
            <Header/>
        </div>
        <div class="team">
            <MemberCard
                name="Pavel Berniak"
                position="Założyciel Crypto Dive"
                photoUrl="../src/assets/photoPavel.png"
                instagramUrl="https://instagram.com/pavelberniak"
                telegramUrl="https://t.me/pavelberniak"
            />
            <MemberCard
                name="Vladyslav Zaker"
                position="Redaktor i resercher"
                photoUrl="../src/assets/photoVladyslav.png"
                instagramUrl="https://instagram.com/vladyslavzaker"
                telegramUrl="https://t.me/vladyslavzaker"
            />
            <MemberCard
                name="Maksim Slysh"
                position="Content manager"
                photoUrl="../src/assets/photoMaksim.png"
                instagramUrl="https://instagram.com/maksim"
                telegramUrl="https://t.me/maksim"
            />
        </div>
    </div>
</template>

<style scoped>
.Page-fourth {
    min-height: 100vh;
}

.team {
    display: flex;
    flex-direction: row;
    gap: 3vw;
    justify-content: space-around;
    align-items: flex-start;
    flex-wrap: wrap;
    margin: 50px 128px 0 128px;
    padding-bottom: 40px;
}

</style>
