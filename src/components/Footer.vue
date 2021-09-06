<template>
<footer>

    
        
           <div class="wrapper container">
        
               <div class="links">
                   <div class="menu">
                       <h3>
                           DC Comics
                       </h3>
                       <ul>
                           <li><a href="">Characters</a></li>
                           <li><a href="">Comics</a></li>
                           <li><a href="">Movies</a></li>
                           <li><a href="">TV</a></li>
                           <li><a href="">Games</a></li>
                           <li><a href="">Videos</a></li>
                           <li><a href="">News</a></li>
                       </ul>
                       <h3>
                           Shop
                       </h3>
                       <ul>
                           <li><a href="">Characters</a></li>
                           <li><a href="">Movies</a></li>
        
                       </ul>
                   </div>
                    <div class="menu">
                         <h3>
                           DC
                       </h3>
                       <ul>
                           <li><a href="">Terms of Use</a></li>
                           <li><a href="">Privacy Policy(New)</a></li>
                           <li><a href="">Ad Choices</a></li>
                           <li><a href="">Advertising</a></li>
                           <li><a href="">Jobs</a></li>
                           <li><a href="">Subscriptions</a></li>
                           <li><a href="">Talent Workshops</a></li>
                           <li><a href="">CPSC Certificates</a></li>
                           <li><a href="">Ratings</a></li>
                           <li><a href="">Shop Help</a></li>
                           <li><a href="">Contact Us</a></li>

                       </ul>
                   </div> 
                   <div class="menu">
                         <h3>
                           Sites
                       </h3>
                       <ul>
                           <li><a href="">DC</a></li>
                           <li><a href="">Mad Magazine</a></li>
                           <li><a href="">DC Kids</a></li>
                           <li><a href="">DC Universe</a></li>
                           <li><a href="">DC Power Visa</a></li>
                       </ul>
                   </div> 
               </div>
               
               <div class="logo">
                   <img src="../assets/img/dc-logo-bg.png" alt="Dc-logo">
               </div>
           </div>
    
    
    



</footer>
  
</template>

<script>
export default {
    name:'Footer'

}
</script>

<style scooped>

footer{
    background-image: url('../assets/img/footer-bg.jpg');
    height: 400px;
    background-size: cover;
    color: white;
    display: flex;
    overflow: hidden;
}

.wrapper{
    width: 100%;
    display: flex;
    justify-content: space-between;

}

.logo{
    align-self: center;
}

ul{
    list-style-type: none;
}

ul li {
    margin: 5px 0 ;

}

ul li a {
    text-decoration: none;
    color: lightgrey;
    
}

.links{
    padding:10px;
    height: 100%;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    width: 40%;
}

.menu h3{
    margin: 10px 0; 
    text-transform: uppercase;
    font-weight: bold;
}


 




</style>