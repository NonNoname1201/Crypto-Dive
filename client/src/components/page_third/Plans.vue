<script setup>

</script>

<template>
  <section class="header">
    <h1>Kup subskypcję w najlepszej cenie</h1>
    <h4>Cena subskrypcji rośnie z każdą większa aktualizacją</h4>
  </section>
  <section class="description-container">
    <div class="description-item">
      <div class="title">
        Dive Club<br>1 miesiąc
      </div>
      <div class="description">
        <ul>
          <li>1x w tygodniu</li>
          <li>1x w weekend</li>
          <li>1x w miesiącu</li>
        </ul>
      </div>
      <div class="price">
        199 ZŁ
      </div>
    </div>
    <div class="description-item">
      <div class="title">
        Dive Club VIP<br>6 miesiące
      </div>
      <div class="description">
        <ul>
          <li>2x w tygodniu</li>
          <li>2x w weekend</li>
          <li>2x w miesiącu</li>
        </ul>
      </div>
      <div class="price">
        999 ZŁ
      </div>
    </div>
    <div class="description-item">
      <div class="title">
        Dive Club Premium<br>&infin;
      </div>
      <div class="description">
        <ul>
          <li>3x w tygodniu</li>
          <li>3x w weekend</li>
          <li>3x w miesiącu</li>
        </ul>
      </div>
      <div class="price">
        2999 ZŁ
      </div>
    </div>
  </section>

</template>

<style scoped>
.header {
  height: 20vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.description-container {
  height: 80vh;
  display: flex;
}

.description-item {
  flex: 1;
  margin: 0 3vw 3vw 3vw;
  border: 1px solid #333;
}
</style>