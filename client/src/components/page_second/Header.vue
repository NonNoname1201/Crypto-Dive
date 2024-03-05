<script setup>

</script>

<script>
export default {
  data() {
    return {
    }
  },
  mounted() {
  }
}
</script>

<template>
  <div class="header">
      <p class="pageName" ref="pageName">Nasz ekosystem</p>
  </div>
</template>

<style scoped>
.header {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 60px;
}

.pageName {
  font-size: 50px;
  font-weight: 700;
  line-height: 61px;

  padding-bottom: 14px;
  background: linear-gradient(270deg, #BD00FF 0%, #0047FF 53%, #31FA0B 100%);
  border: 0;
  position: relative;
  z-index: 1;
}

.pageName:before {
  content: "";
  display: block;
  height: 69px;
  width: 100%;
  background: black;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}

</style>