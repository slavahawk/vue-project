<script setup></script>

<template>
  <div class="cards">
    <div>
      <div class="card__dop">
        <button>
          <img src="@/assets/img/mobile.svg" alt="favorite" />
        </button>
        <button>
          <img src="@/assets/img/mobile.svg" alt="favorite" />
        </button>
      </div>

      <div class="card__image">
        <img src="@/assets/img/mobile.svg" alt="" />
      </div>
      <h4>Цепная пила PATRIOT ESP 1614</h4>
      <div class="sale">Скидка при онлайн оплате 10 000 ₽</div>
      <span class="tags">
        <div class="tag">Хит продаж</div>
        <div class="tag">Рассрочка</div>
        <img src="@/assets/img/mobile.svg" alt="" />
      </span>
    </div>
    <div class="wid">
      <div class="cence">
        <div>
          <div>
            <div class="cena">Розничная цена:</div>
            <div class="cena__nomber">832 920 ₽</div>
          </div>
        </div>
        <div>
          <div>
            <div class="cena">Клубная цена:</div>
            <div class="cena__nomber">322 220 ₽</div>
          </div>
        </div>
      </div>

      <div class="hochu">
        <img src="@/assets/img/mobile.svg" alt="" />
        <div>Хочу клубную цену и до 1199 бонусов</div>
      </div>
      <button class="buy">
        <img src="@/assets/img/mobile.svg" alt="" />
        <div style="font-weight: 500">В корзину</div>
      </button>

      <div class="info__hover">asds</div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.cards {
  background-color: var(--white);
  border: 1px solid #f2f2f2;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  border-radius: 12px;
  position: relative;
  padding: 16px;
  min-height: 570px;

  &:hover {
    .info__hover {
      display: block;
    }
  }

  //   img {
  //     margin: 40px;
  //   }
  //   div {
  //     // margin: 15px;
  //   }
}

.card__image {
  padding: 37px 66px 37px;
  img {
    width: 100%;
  }
}
h4 {
  font-size: 20px;
  font-weight: 400;
  margin: 0 0 12px;
}
.sale {
  background: #fff0f8;
  padding: 4px 12px 4px 12px;
  gap: 10px;
  color: #ab015b;
  border-radius: 19px;
  margin: 0 0 12px;
}
.tags {
  display: flex;

  .tag {
    background: #daf5ff;
    padding: 4px 12px 4px 12px;
    border-radius: 19px;
    gap: 10px;
  }
}

.card__dop {
  position: absolute;
  top: 15px;
  right: 15px;
  display: flex;
  flex-direction: column;
  gap: 4px;

  button {
    border: none;
    background: transparent;
    img {
      width: 24px;
      height: 24px;
    }
  }
}

.info__hover {
  display: none;
}
.wid {
  display: flex;
  flex-direction: column;
  gap: 32px;
}
.cence {
  display: flex;
  flex-direction: row;
  gap: 40px;
}
.cena {
  font-size: 14px;
}
.cena__nomber {
  font-size: 26px;
  font-weight: 500;
}
.hochu {
  color: #1956b7;
  text-decoration: underline;
  text-decoration-style: dotted;
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 3px;
}
.buy {
  background-color: var(--yellow);
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  border-radius: 8px;
  border: none;
  gap: 8px;
  padding: 12px 48px 12px 48px;
}
</style>
