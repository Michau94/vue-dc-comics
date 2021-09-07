<template>
  <div class="bonus">
    <div class=" container wrapper">
      <div class="card" v-for="(card, index) in images" :key="index">
        <figure>
          <img :src="card.path" alt="DigitalComics" />
        </figure>
        <span>{{ card.text }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Bonus",
  data() {
    return {
      images: [
        {
          path: require("@/assets/img/buy-comics-digital-comics.png"),
          text: "Digital Comics",
        },
        {
          path: require("@/assets/img/buy-comics-merchandise.png"),
          text: "DC Merchandise",
        },
        {
          path: require("@/assets/img/buy-comics-subscriptions.png"),
          text: "Subscription",
        },
        {
          path: require("@/assets/img/buy-comics-shop-locator.png"),
          text: "Comic Shop Locator",
        },
        {
          path: require("../assets/img/buy-dc-power-visa.svg"),
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars.scss";

.bonus {
  height: 200px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  background-color: $base-color;
}

.card {
  display: flex;
  align-items: center;

  img {
    width: 100%;
    height: 100px;
    padding: 10px;
  }

  span {
    color: $text-main;
    font-weight: 500;
  }
}
</style>
