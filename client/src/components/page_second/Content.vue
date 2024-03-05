<script setup>
import IconCore from "@/components/icons/page_second/IconCore.vue";
import IconNews from "@/components/icons/page_second/IconNews.vue";
import IconMoney from "@/components/icons/page_second/IconMoney.vue";
import IconMember from "@/components/icons/page_second/IconMember.vue";
import IconStudent from "@/components/icons/page_second/IconStudent.vue";
</script>

<template>
<div class="Content">
  <div class="core"><IconCore/></div>
  <div class="images">
    <IconNews/>
    <IconMoney/>
    <IconMember/>
    <IconStudent/>
  </div>
</div>

</template>

<style scoped>
.Content {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 80vh;
  z-index: -1;
}

.core {
  margin: 0 auto;
  width: 60%;
  height: 100%;
  svg {
    width: 100%;
    height: 100%;
  }
}

.images {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  gap: 160px;
  width: 79%;
  height: 90%;
  margin: 0;
  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }

  position: absolute;
  background: transparent;
}
</style>