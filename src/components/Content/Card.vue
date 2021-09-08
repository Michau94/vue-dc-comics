<template>
  <div class="container">
    <div class="button">
      Current Series
    </div>
    <div class="card" v-for="(card, index) in data" :key="index">
      <figure>
        <img :src="card.thumb" :alt="card.series" />
      </figure>
      <figcaption>{{ card.series }}</figcaption>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["data"],
};
</script>

<style lang="scss" scoped>
@import "../../assets/sass/_vars.scss";
@import "../../assets/sass/_mixin.scss";

.container {
  @include center("both");
  flex-wrap: wrap;
  position: relative;
  margin: 10px 0;
  .card {
    display: flex;
    flex-direction: column;
    flex-basis: calc(100% / 6);
    padding: 10px;
    height: 350px;

    img {
      width: 100%;
      height: 250px;
    }

    figcaption {
      color: white;
      text-transform: uppercase;
      padding: 3px;
    }
  }
}

.button {
  position: absolute;
  top: -60px;
  left: 10px;
  color: white;
  font-size: 2rem;
  font-weight: bold;
  padding: 10px;
  background-color: $base-color;
}
</style>
