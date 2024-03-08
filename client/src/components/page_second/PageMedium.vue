<script setup>
import SkeletonMedium from "@/components/icons/page_second/medium/SkeletonMedium.vue";
import IconMemberThin from "@/components/icons/page_second/thin/IconThinMember.vue";
import IconStudentThin from "@/components/icons/page_second/thin/IconThinStudent.vue";
import IconMoneyThin from "@/components/icons/page_second/thin/IconThinMoney.vue";
import IconNewsThin from "@/components/icons/page_second/thin/IconThinNews.vue";
</script>

<template>
  <div class="Content">
    <div class="skeleton-medium">
      <SkeletonMedium/>
    </div>
<!--    <div class="icon-container-medium">-->
<!--      <div class="sub-container-icon">-->
<!--        <div class="sub-sub-container-icon">-->
<!--          <div class="icon-medium icon-news-medium">-->
<!--            <IconNewsThin/>-->
<!--          </div>-->
<!--          <div class="icon-medium icon-money-medium">-->
<!--            <IconMoneyThin/>-->
<!--          </div>-->
<!--        </div>-->
<!--        <div class="sub-sub-container-icon">-->
<!--        </div>-->
<!--      </div>-->
<!--      <div class="sub-container-icon">-->
<!--        <div class="sub-sub-container-icon">-->
<!--        </div>-->
<!--        <div class="sub-sub-container-icon">-->
<!--          <div class="icon-medium icon-member-medium">-->
<!--            <IconMemberThin/>-->
<!--          </div>-->
<!--          <div class="icon-medium icon-student-medium">-->
<!--            <IconStudentThin/>-->
<!--          </div>-->
<!--        </div>-->
<!--      </div>-->
<!--    </div>-->
<!--    <div class="icon-container-medium" ref="iconContainer">-->
<!--      <div class="icon-medium icon-news-medium">-->
<!--        <IconNewsThin/>-->
<!--      </div>-->
<!--      <div class="icon-medium icon-money-medium">-->
<!--        <IconMoneyThin/>-->
<!--      </div>-->
<!--      <div class="icon-medium icon-member-medium">-->
<!--        <IconMemberThin/>-->
<!--      </div>-->
<!--      <div class="icon-medium icon-student-medium">-->
<!--        <IconStudentThin/>-->
<!--      </div>-->
<!--    </div>-->
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
  position: absolute;
  background: transparent;
  width: 100%;
  height: 80vh;

  display: flex;
  justify-content: center;
  gap: 3vw;
  flex-grow: 1;
}

.sub-container-icon {
  background: transparent;
  width : 35.7vw;
  height: 100%;
  display: flex;
  flex-direction: column;
}

.sub-sub-container-icon {
  background: transparent;
  width: 100%;
  height: 50%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.icon-medium {
  position: absolute;

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
  //top: 0.7%;
  //left: 1.5vw;
}

.icon-money-medium {
  --svg-size: 60%;
  width: var(--svg-size);
  height: var(--svg-size);
  //top: 11%;
  //left: -0.5vw;
}

.icon-member-medium {
  --svg-size: 43%;
  width: var(--svg-size);
  height: var(--svg-size);
  //bottom: 22%;
  //right: 3.5vw;
}

.icon-student-medium {
  --svg-size: 57%;
  width: var(--svg-size);
  height: var(--svg-size);
  //bottom: -2%;
  //right: 1vw;
}
</style>