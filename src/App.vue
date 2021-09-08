<template>
  <div id="app">
    <Header />
    <main>
      <Jumbo />
      <Content />
      <Bonus />
    </main>
    <Footer />
    <Media />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Content from "./components/Content.vue";
import Bonus from "./components/Bonus.vue";
import Footer from "./components/Footer.vue";
import Media from "./components/Media.vue";
import Jumbo from "./components/Jumbo.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Footer,
    Media,
    Bonus,
    Jumbo,
  },
};
</script>

<style lang="scss">
@import "./assets/sass/style.scss";
</style>
