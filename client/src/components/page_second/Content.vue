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
    <div class="icon left-top-icon">
      <IconNews/>
    </div>
    <div class="right-top-icon icon">
      <IconMoney/>
    </div>
    <div class="left-bottom-icon icon">
      <IconMember/>
    </div>
    <div class="right-bottom-icon icon">
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
}

.core {
  width: 60%;
  height: 100%;
  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }
  background: transparent;
}

.icon-container {
  position: absolute;
  background: transparent;
  width: 100%;
  height: 100%;
}

.icon{
  --svg-size: 20%;
  --move-up: 28vh;
  --move-left: 22vw;
  position: absolute;
  top: calc(50% - var(--move-up));
  left: calc(50% - var(--move-left));
  width: var(--svg-size);
  height: var(--svg-size);
  transform: translate(-50%, -50%);
  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }
  background: transparent;
}

.left-top-icon{
  --move-up: 28vh;
  --move-left: 22vw;
}

.right-top-icon{
  --move-up: 28vh;
  --move-left: -22vw;
}
.right-bottom-icon{
  --move-up: -28vh;
  --move-left: -22vw;
}
.left-bottom-icon{
  --move-up: -28vh;
  --move-left: 22vw;
}
</style>