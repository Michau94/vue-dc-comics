<template>
<div class="media">
    
      <div class="wrapper container">
          <div class="button">
              Sign-Up Now!
              
          </div>
    
          <div class="social">
            <h3>Follow Us</h3>
            <div><img src="../assets/img/footer-facebook.png" alt="FB"></div>
            <div><img src="../assets/img/footer-pinterest.png" alt="Pinterest"></div>
            <div><img src="../assets/img/footer-periscope.png" alt="Periscope"></div>
            <div><img src="../assets/img/footer-twitter.png" alt="Twitter"></div>
            <img src="../assets/img/footer-youtube.png" alt="Youtube">
    
          </div>
    
    
    
      </div>
</div>
</template>

<script>
export default {
    name:'Media',

}
</script>

<style scoped>

.media {
    background-color: #242424;
    height: 100px;
}
.wrapper{
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.social{
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    width: 30%;
}

.social h3{
    text-transform: uppercase;
    font-weight: 500;
    color:#0C7CEC;
}

.button{
    padding: 10px 15px;
    border: 1px solid #0C7CEC;
    height: 50px;
    display: flex;
    align-items: center;
    color:white; 
    font-weight: bold;
    text-transform: uppercase;
   
}

.wrapper{
    display:flex;
    align-items: center;
    justify-content: space-between;
}



</style>