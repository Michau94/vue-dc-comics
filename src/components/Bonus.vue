<template>
  <div class="bonus">
      
          <div class=" container wrapper">
              <div class="card">
                  <figure><img src="../assets/img/buy-comics-digital-comics.png" alt="DigitalComics"></figure>
                  <span>Digital Comics</span>
              </div>
              <div class="card">
                  <figure><img src="../assets/img/buy-comics-merchandise.png" alt="DigitalComics"></figure>
                  <span>DC Merchandise</span>
              </div>
              <div class="card">
                  <figure><img src="../assets/img/buy-comics-subscriptions.png" alt="DigitalComics"></figure>
                  <span>Subscription</span>
              </div>
              <div class="card">
                  <figure><img src="../assets/img/buy-comics-shop-locator.png" alt="DigitalComics"></figure>
                  <span>Comic Shop Locator</span>
              </div>
              <div class="card">
                  <figure><img src="../assets/img/buy-dc-power-visa.svg" alt="DigitalComics"></figure>
                  <span>DC Power Visa</span>
              </div>
          </div>
  </div>
  
</template>

<script>
export default {
    name:'Bonus'

}
</script>

<style scoped>

.wrapper{
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.bonus{
    height: 200px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    background-color: dodgerblue;
}

.card{
    display: flex;
    align-items: center;
    
}

.card img{
    width: 100%;
    height: 100px;
    padding: 10px; 
}

.card span{
    color: #fff;
    font-weight: 500;
}


</style>


