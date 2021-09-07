<template>
  <div id="app">
    <Header />
    <main>
      <Content />
      <Bonus />
    </main>
    <Footer />
    <Media />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Content from "@/components/Content.vue";
import Footer from "@/components/Footer.vue";
import Media from "@/components/Media.vue";
import Bonus from "@/components/Bonus.vue";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Footer,
    Media,
    Bonus,
  },
};
</script>

<style lang="scss">
@import "@/assets/sass/style.scss";
</style>
