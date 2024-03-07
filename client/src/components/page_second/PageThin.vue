<script setup>
import SkeletonThin from "@/components/icons/page_second/thin/SkeletonThin.vue";
import IconMemberThin from "@/components/icons/page_second/thin/IconMemberThin.vue";
import IconNewsThin from "@/components/icons/page_second/thin/IconNewsThin.vue";
import IconMoneyThin from "@/components/icons/page_second/thin/IconMoneyThin.vue";
import IconStudentThin from "@/components/icons/page_second/thin/IconStudentThin.vue";
</script>

<template>
  <div class="Content">
    <div class="skeleton-thin"><SkeletonThin/></div>
    <div class="icon-container-thin">
      <div class="icon-thin icon-news-thin">
        <IconNewsThin/>
      </div>
      <div class="icon-thin icon-money-thin">
        <IconMoneyThin/>
      </div>
      <div class="icon-thin icon-member-thin">
        <IconMemberThin/>
      </div>
      <div class="icon-thin icon-student-thin">
        <IconStudentThin/>
      </div>
    </div>
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

.icon-news-thin{
  --svg-size: 60%;
  width: var(--svg-size);
  height: var(--svg-size);
  top: -6%;
}

.icon-money-thin{
  --svg-size: 65%;
  width: var(--svg-size);
  height: var(--svg-size);
  top: 10%;
}

.icon-member-thin{
  --svg-size: 53%;
  width: var(--svg-size);
  height: var(--svg-size);
  bottom: 12%;
}

.icon-student-thin{
  --svg-size: 79%;
  width: var(--svg-size);
  height: var(--svg-size);
  bottom: -20%;
}


</style>