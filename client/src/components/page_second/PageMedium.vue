<script setup>
import SkeletonMedium from "@/components/icons/page_second/medium/SkeletonMedium.vue";
import IconMemberThin from "@/components/icons/page_second/thin/IconMemberThin.vue";
import IconStudentThin from "@/components/icons/page_second/thin/IconStudentThin.vue";
import IconMoneyThin from "@/components/icons/page_second/thin/IconMoneyThin.vue";
import IconNewsThin from "@/components/icons/page_second/thin/IconNewsThin.vue";
</script>

<template>
  <div class="Content">
    <div class="skeleton-medium">
      <SkeletonMedium/>
    </div>
    <div class="icon-container-medium" ref="iconContainer">
      <div class="icon-medium icon-news-medium">
        <IconNewsThin/>
      </div>
      <div class="icon-medium icon-money-medium">
        <IconMoneyThin/>
      </div>
      <div class="icon-medium icon-member-medium">
        <IconMemberThin/>
      </div>
      <div class="icon-medium icon-student-medium">
        <IconStudentThin/>
      </div>
    </div>
  </div>
</template>

<style scoped>
/*min 670px max 1024px*/
.Content {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 80vh;
}

.skeleton-medium {
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

.icon-container-medium {
  background: transparent;
  position: absolute;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 60%;
  height: 100%;

}

.icon-medium {
  position: ABSOLUTE;

  svg {
    width: 100%;
    height: 100%;
    background: transparent;
  }

  background: transparent;
}

.icon-news-medium {
  --svg-size: 50%;
  width: var(--svg-size);
  height: var(--svg-size);
  top: 0.7%;
  left: 1.5vw;
}

.icon-money-medium {
  --svg-size: 60%;
  width: var(--svg-size);
  height: var(--svg-size);
  top: 11%;
  left: -0.5vw;
}

.icon-member-medium {
  --svg-size: 43%;
  width: var(--svg-size);
  height: var(--svg-size);
  bottom: 22%;
  right: 3.5vw;
}

.icon-student-medium {
  --svg-size: 57%;
  width: var(--svg-size);
  height: var(--svg-size);
  bottom: -2%;
  right: 1vw;
}
</style>