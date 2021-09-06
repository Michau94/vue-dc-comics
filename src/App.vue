<template>
  <div id="app">
    <Header/>
    <Content/>
    <Footer/>
    <Media/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Content from '@/components/Content.vue'
import Footer from '@/components/Footer.vue'
import Media from '@/components/Media.vue'


export default {
  name: "App",
  components: {
    Header,
    Content,
    Footer,
    Media
    
  },
  
}
</script>

<style lang="scss">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  font-family: 'Raleway', sans-serif;
  
}

.container{
  max-width: 1500px;
  margin: 0 auto; 
  height: 100%;
}
</style>
