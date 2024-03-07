<script setup>
import IconCore from "@/components/icons/page_second/wide/SkeletonWide.vue";
import IconStudent from "@/components/icons/page_second/wide/IconStudentWide.vue";
import IconMember from "@/components/icons/page_second/wide/IconMemberWide.vue";
import IconMoney from "@/components/icons/page_second/wide/IconMoneyWide.vue";
import BgText from "@/components/icons/page_second/wide/BgText.vue";
import IconNews from "@/components/icons/page_second/wide/IconNewsWide.vue";
</script>

<template>
  <div class="Content">
    <div class="bg-text"><BgText/></div>
    <div class="skeleton-wide"><IconCore/></div>
    <div class="icon-container-wide">
      <div class="icon-wide icon-news-wide">
        <IconNews/>
      </div>
      <div class="icon-wide icon-money-wide">
        <IconMoney/>
      </div>
      <div class="icon-wide icon-member-wide">
        <IconMember/>
      </div>
      <div class="icon-wide icon-student-wide">
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

.bg-text {
  position: absolute;
  width: 90%;
  height: 100%;
  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }
  background: transparent;
}

.skeleton-wide {
  padding-bottom: 2vh;
  align-items: center;
  width: 70%;
  height: 100%;
  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }
  background: transparent;
}

.icon-container-wide {
  position: absolute;
  background: transparent;
  width: 100%;
  height: 100%;
}

.icon-wide{
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

.icon-news-wide{
  --move-up: 15.7vw;
  --move-left: 26vw;
}
.icon-money-wide{
  --move-up: 15.7vw;
  --move-left: -26vw;
}
.icon-student-wide{
  --move-up: -15.3vw;
  --move-left: -26vw;
}
.icon-member-wide{
  --move-up: -15.3vw;
  --move-left: 26vw;
}
</style>