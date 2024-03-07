<script setup>
import Blocks from "@/components/icons/page_second/medium/SkeletonMediumBlocks.vue";
import Arks from "@/components/icons/page_second/medium/SkeletonMediumArks.vue";
import LogoBubbles from "@/components/icons/page_second/medium/SkeletonMediumLogoBubbes.vue";
import Logos from "@/components/icons/page_second/medium/SkeletonMediumLogo.vue";
import IconMediumMember from "@/components/icons/page_second/medium/IconMediumMember.vue";
import IconMediumStudent from "@/components/icons/page_second/medium/IconMediumStudent.vue";
import IconMediumNews from "@/components/icons/page_second/medium/IconMediumNews.vue";
import IconMediumMoney from "@/components/icons/page_second/medium/IconMediumMoney.vue";
</script>

<template>
  <div class="skeleton-medium">
    <div class="skeleton-element">
      <LogoBubbles />
    </div>
    <div class="skeleton-element">
      <Blocks />
    </div>
    <div class="skeleton-element">
      <Arks />
    </div>
    <div class="skeleton-element">
      <Logos />
    </div>
    <div class="skeleton-element">
      <IconMediumMember />
    </div>
    <div class="skeleton-element">
      <IconMediumStudent />
    </div>
    <div class="skeleton-element">
      <IconMediumNews />
    </div>
    <div class="skeleton-element">
      <IconMediumMoney />
    </div>
  </div>
</template>

<style scoped>
  .skeleton-medium {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 100%;
  }

  .skeleton-element {
    background: transparent;
    position: absolute;
    svg{
      background: transparent;
      width: 100%;
      height: 100%;
    }
  }
</style>