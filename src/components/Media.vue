<template>
  <div class="media">
    <div class="wrapper container">
      <div class="button">
        <a href="">Sign-Up Now!</a>
      </div>

      <div class="social">
        <h3>Follow Us</h3>

        <div>
          <a href=""><img src="../assets/img/footer-facebook.png" alt="FB"/></a>
        </div>
        <div>
          <a href=""
            ><img src="../assets/img/footer-pinterest.png" alt="Pinterest"
          /></a>
        </div>
        <div>
          <a href=""
            ><img src="../assets/img/footer-periscope.png" alt="Periscope"
          /></a>
        </div>
        <div>
          <a href=""
            ><img src="../assets/img/footer-twitter.png" alt="Twitter"
          /></a>
        </div>
        <div>
          <a href=""
            ><img src="../assets/img/footer-youtube.png" alt="Youtube"
          /></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Media",
};
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars";

.media {
  background-color: #242424;
  height: 100px;
}

.social {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  width: 30%;
  h3 {
    text-transform: uppercase;
    font-weight: 500;
    color: $base-color;
  }
}

.social a,
a {
  display: block;
  text-decoration: none;
  color: #fff;
}

.button {
  padding: 10px 15px;
  border: 1px solid #0c7cec;
  height: 50px;
  display: flex;
  align-items: center;
  color: white;
  font-weight: bold;
  text-transform: uppercase;
}

.wrapper {
  align-items: center;
}
</style>
