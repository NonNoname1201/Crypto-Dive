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
  <div class="icon-container">
    <div class="left-top-icon icon">
      <IconNews/>
    </div>
    <div class="right-top-icon icon">
      <IconMoney/>
    </div>
    <div class="right-bottom-icon icon">
      <IconMember/>
    </div>
    <div class="left-bottom-icon icon">
      <IconStudent/>
    </div>
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
  width: 60%;
  height: 100%;
  svg {
    width: 100%;
    height: 100%;
  }
}

.icon-container {
  position: absolute;
  background: transparent;

}

.icon{
  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }
  background: transparent;
}

.left-top-icon{
  position: relative;
  bottom: 28vh;
  right: 22vw;
  z-index: 1;
}

.right-top-icon{
  position: relative;
  bottom: 28vh;
  left: 22vw;
  z-index: 2;
}
.right-bottom-icon{
  position: relative;
  top: 28vh;
  left: 22vw;
  z-index: 3;
}
.left-bottom-icon{
  position: relative;
  top: -28vh;
  left: -22vw;
  z-index: 4;
}
</style>