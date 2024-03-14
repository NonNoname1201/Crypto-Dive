<script setup>

import Header from "@/components/page_fourth/Header.vue";
import MemberCardPavel from "@/components/page_fourth/MemberCardPavel.vue";
import MemberCardVladyslav from "@/components/page_fourth/MemberCardVladyslav.vue";
import MemberCardMaksim from "@/components/page_fourth/MemberCardMaksim.vue";
</script>

<template>
    <div class="Page-fourth page">
        <div class="header">
            <Header/>
        </div>
        <div class="team">
            <div class="teamMember">
                <MemberCardPavel/>
            </div>
            <div class="teamMember">
                <MemberCardVladyslav/>
            </div>
            <div class="teamMember">
                <MemberCardMaksim/>
            </div>
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
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    margin: 0 128px;
    padding-bottom: 40px;
}

.teamMember {
    margin: 0 16px 32px 16px;
    transition: 0.3s;
}

.teamMember:hover {
    transform: scale(1.05);
    transition: 0.3s;
}

</style>
