<script setup>
import Card from "./Card.vue";
</script>

<template>
  <div class="card">
    <div class="card__content">
      <div class="card__head">
        <span style="font-size: 40px; font-weight: 500">Сезонные товары</span>
        <div>
          <span class="links">
            <div class="pili">
              <div>Бензиновые пилы 12</div>
              <img src="@/assets/img/mobile.svg" alt="" />
            </div>
            <div class="sens">Пылесосы садовые 221</div>
            <div class="sens">Мотоблоки 11</div>
            <div class="sens">Черенки, рукоятки 45</div>
          </span>
          <div class="icon">
            <img src="@/assets/img/mobile.svg" alt="" />
            <img src="@/assets/img/mobile.svg" alt="" />
          </div>
        </div>
        <div class="hol">
          <Card />
          <Card />
          <Card />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.card {
  background: #f4f5f5;
  padding: 40px auto;
  margin: 40px auto;
}
.card__content {
  display: flex;

  max-width: 1920px;
  margin: 0 auto;
  width: 100%;
}

.card__head {
  padding: 0 40px;
}
.links {
  display: flex;
  margin: 30px auto;
  gap: 10px;
}
.sens {
  background: var(--white);
  padding: 5px;
  border-radius: 20px;
  display: flex;
  justify-content: space-between;
}
.pili {
  background: #ffee00;
  padding: 5px;
  border-radius: 20px;
  display: flex;
  justify-content: flex-start;
}
.icon {
  display: flex;
  align-items: center;
}
.icons {
  display: flex;
  align-items: center;
}
.hol {
  display: flex;
  justify-content: space-between;
}
</style>
