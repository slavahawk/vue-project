<script setup>
import { ref } from "vue";

const sale = ref("До окончания акции: 18:12:41");
</script>

<template>
  <main class="main">
    <div class="main__content">
      <div class="main__links">
        <div class="main__one link__card">
          <span style="font-weight: 500; font-size: 25px; line-height: 26px">
            Популярные категории
          </span>
          <div
            style="display: flex; align-items: center"
            @click="sale = 'asdasdasd'"
          >
            <img src="@/assets/img/mobile.svg" alt="" />
            <span>Телефоны и планшеты</span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Компьютеры и ноутбуки </span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Оргтехника и сети </span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Теле, аудио, фото</span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Для автомобиля </span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Техника для дома </span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Техника для кухни </span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Красота и здоровье </span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Инструмент </span>
          </div>
          <div style="display: flex; align-items: center">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span> Велосипеды и спорт </span>
          </div>
        </div>

        <div class="main__two link__card">
          <img src="@/assets/img/mobile.svg" alt="" />
          <span> Уцененные товары</span>
        </div>
      </div>

      <div class="main__baner">
        <div class="main__ban">
          <img src="@/assets/img/mobile.svg" alt="" />
        </div>

        <div
          style="
            display: flex;
            justify-content: flex-start;
            font-weight: 500;
            font-size: 40px;
            line-height: 52px;
          "
        >
          Акции
        </div>
        <div class="main__baners">
          <div class="card__banner">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span>{{ sale }}</span>
          </div>
          <div class="card__banner">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span>{{ sale }}</span>
          </div>
          <div class="card__banner">
            <img src="@/assets/img/mobile.svg" alt="" />
            <span>{{ sale }}</span>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<style lang="scss">
.main {
  background: var(--white);
  display: flex;
}

.main__content {
  display: flex;
  max-width: 1920px;
  margin: 0 auto;
  width: 100%;
  gap: 20px;
  padding: 13px;
}
.main__links {
  display: flex;
  flex-direction: column;
  flex: 0 0 360px;
  @media screen and (max-width: 935px) {
    display: none;
  }
}

.link__card {
  border: 1px solid rgb(206, 205, 205);
  border-radius: 12px;
  padding: 24px 27px 24px 47px;
  display: flex;
}

.main__one {
  flex-direction: column;
  gap: 24px;
}
.main__two {
  align-items: center;
  margin: 40px 0 0;
}
.main__baner {
  display: flex;
  flex-direction: column;
  width: 100%;
}
.main__ban {
  @media screen and (max-width: 935px) {
    width: 100%;
    // height: 84px;
  }
  img {
    width: 100%;
  }
}
.main__baners {
  display: flex;
  gap: 20px;
}

.card__banner {
  border: 1px solid rgb(206, 205, 205);
  border-radius: 12px;
  width: 100%;

  img {
    width: 100%;
  }

  span {
    padding: 10px;
    font-weight: 500;
    display: block;
  }
}
</style>
