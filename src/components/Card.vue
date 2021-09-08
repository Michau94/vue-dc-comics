<template>
  <div class="container">
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
.container {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
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
</style>
