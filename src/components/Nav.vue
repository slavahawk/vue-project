<script setup></script>

<template>
  <nav class="nav">
    <div class="nav__content">
      <div style="display: flex; gap: 20px">
        <div class="nav__logo">
          <img s src="@/assets/img/mobile.svg" alt="" />
        </div>
        <button class="nav__menu">
          <img src="@/assets/img/mobile.svg" alt="" />
          <span>КАТАЛОГ</span>
        </button>

        <label for="search" class="nav__poisk">
          <input id="search" type="assept" placeholder="Поиск по сайту" />
          <img src="@/assets/img/mobile.svg" alt="" />
        </label>
      </div>

      <div class="nav__click">
        <div
          style="
            display: flex;
            justify-content: space-around;
            align-items: flex-end;
          "
        >
          <img src="@/assets/img/mobile.svg" alt="" />
          <span>Статус заказа</span>
        </div>
        <div
          style="
            display: flex;
            justify-content: space-around;
            align-items: center;
          "
        >
          <img src="@/assets/img/mobile.svg" alt="" />
          <span>Сравнение</span>
        </div>
        <div
          style="
            display: flex;
            justify-content: space-around;
            align-items: center;
          "
        >
          <img src="@/assets/img/mobile.svg" alt="" />
          <span>Избраное</span>
        </div>
        <div
          style="
            display: flex;
            justify-content: space-around;
            align-items: center;
          "
        >
          <img src="@/assets/img/mobile.svg" alt="" />
          <span>34 920</span>
        </div>
        <div
          style="
            display: flex;
            justify-content: space-around;
            align-items: center;
          "
        >
          <img src="@/assets/img/mobile.svg" alt="" />
          <span>Вход | Регистрация</span>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped lang="scss">
.nav {
  background: var(--white);
  @media screen and (max-width: 935px) {
    display: flex;
    justify-content: space-around;
    width: 100%;
  }
}
.nav__content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1920px;
  width: 100%;
  margin: 0 auto;

  padding: 13px;
}
.nav__links {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
}

.nav__menu {
  background: var(--yellow);
  padding: 4px 24px 4px 24px;
  border-radius: 4px;
  display: flex;
  align-items: center;
  border: none;
  span {
    font-weight: 500;
    @media screen and (max-width: 935px) {
      display: none;
    }
  }
}

.nav__click {
  display: flex;
  gap: 20px;
  @media screen and (max-width: 935px) {
    display: none;
  }

  div {
    gap: 6px;
  }
}

.nav__poisk {
  border: 1px solid black;
  max-width: 470px;
  min-width: 100px;
  display: flex;
  width: 100%;
  input {
    width: 100%;
    height: 40px;
    color: darkgrey;
    border: none;
  }
}
.nav__logo {
  display: flex;
  align-items: center;
  @media screen and (max-width: 976px) {
    display: none;
  }
}
</style>
