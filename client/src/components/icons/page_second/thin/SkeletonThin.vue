<script setup>
import SkeletonThinArks from "@/components/icons/page_second/thin/SkeletonThinArks.vue";
import IconThinNews from "@/components/icons/page_second/thin/IconThinNews.vue";
import IconThinMoney from "@/components/icons/page_second/thin/IconThinMoney.vue";
import IconThinMember from "@/components/icons/page_second/thin/IconThinMember.vue";
import IconThinStudent from "@/components/icons/page_second/thin/IconThinStudent.vue";
import SkeletonThinBlocks from "@/components/icons/page_second/thin/SkeletonThinBlocks.vue";
</script>

<template>
  <div class="skeleton-thin">
    <div class="skeleton-element">
      <SkeletonThinBlocks />
    </div>
    <div class="skeleton-element">
      <SkeletonThinArks />
    </div>
    <div class="skeleton-element">
      <IconThinNews />
    </div>
    <div class="skeleton-element">
      <IconThinMoney />
    </div>
    <div class="skeleton-element">
      <IconThinStudent />
    </div>
    <div class="skeleton-element">
      <IconThinMember />
    </div>
  </div>
</template>

<style scoped>
  .skeleton-thin {
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