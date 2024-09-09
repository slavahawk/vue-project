<script setup></script>

<template>
  <header class="header">
    <div class="header__content">
      <div class="header__links">
        <img class="header__logo" src="@/assets/img/mobile.svg" alt="" />
        <div class="header__link">
          <img src="@/assets/img/mobile.svg" alt="mb" />
          <span>Красноярск</span>
        </div>
        <div class="header__link_">Магазин</div>

        <div class="header__link_">
          <span>Покупателям</span>
          <img src="@/assets/img/mobile.svg" alt="vm" />
        </div>
        <div class="header__link_">
          <span>Компания</span>
          <img src="@/assets/img/mobile.svg" alt="vm" />
        </div>
        <div class="header__link_">
          <span>Организациям</span>
          <img src="@/assets/img/mobile.svg" alt="vm" />
        </div>

        <div class="header__link_">Акции</div>
        <div class="header__link_">Статьи</div>
        <div class="header__link_">Подарочные карты</div>
      </div>

      <div class="header__tel">
        <span style="margin-right: 4px; font-size: 14px; font-weight: 600"
          >8-(800)-775-00-70 доб.3020
        </span>
        <span style="font-size: 12px; font-weight: 0; color: darkgrey"
          >(бесплатно по России)</span
        >
      </div>
    </div>
  </header>
</template>

<style scoped>
.header {
  background: #545050;
  padding: 12px;

  color: aliceblue;
  @media screen and (max-width: 935px) {
    background: var(--white);
    display: flex;
    justify-content: space-around;
  }
}

.header__content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1920px;
  margin: 0 auto;
}
.header__tel {
  display: flex;
  justify-content: space-around;
  @media screen and (max-width: 1200px) {
    display: none;
  }
}

.header__links {
  display: flex;
  justify-content: space-around;
  align-items: center;
  gap: 70px;
}

.header__link {
  display: flex;
  align-items: center;
  gap: 8px;
  @media screen and (max-width: 935px) {
    display: flex;
    justify-content: flex-end;
    color: var(--black);
  }
}

.header__logo {
  display: none;
  @media screen and (max-width: 976px) {
    display: block;
  }
}
.header__link_ {
  @media screen and (max-width: 935px) {
    display: none;
  }
}
</style>
