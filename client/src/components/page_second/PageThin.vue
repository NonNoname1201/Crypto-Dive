<script setup>
import SkeletonThin from "@/components/icons/page_second/thin/SkeletonThin.vue";
</script>

<template>
  <div class="Content">
    <div class="skeleton-thin"><SkeletonThin/></div>
  </div>
</template>

<style scoped>
/*min 430px max 670px*/

.Content {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 80vh;
}

.skeleton-thin {
  padding-top: 5vh;
  align-items: center;
  width: 100%;
  height: 100%;
  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }
  background: transparent;
}

.icon-container-thin{
  padding-top: 5vh;
  background: transparent;
  position: absolute;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 60%;
  height: 100%;

}

.icon-thin{
  position: ABSOLUTE;
  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }
  background: transparent;
}


</style>