<template>
  <section>
    <div class="container">
      <Card :data="DcComics" />
    </div>
    <Button message="Load More" />
  </section>
</template>

<script>
import Card from "./Content/Card.vue";
import Button from "./Content/Button.vue";
import DcComics from "../assets/data/dc-comics.js";

export default {
  name: "Content",
  components: {
    Card,
    Button,
  },
  data() {
    return {
      DcComics,
    };
  },
};
</script>

<style lang="scss" scoped>
section {
  padding: 20px;
  background-color: black;
  text-align: center;
}
</style>
