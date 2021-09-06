<template>
<header>
    <div class="container wrapper">
    <img src="../assets/img/dc-logo.png" alt="Logo">

    <nav>
        <ul>
            <li :class="{active:link.current}" v-for="(link, index) in data" :key="index"><a :href="link.url">{{ link.text }}</a></li>
        </ul>
    </nav>



    </div>

</header>
  
</template>

<script>
export default {
    name:'Header',
    data(){
    return {
      data: [
  {
    text: 'Characters',
    url: '#',
    current: false,
  },
  {
    text: 'Comics',
    url: '#',
    current: true,
  },
  {
    text: 'Movies',
    url: '#',
    current: false,
  },
  {
    text: 'TV',
    url: '#',
    current: false,
  },
  {
    text: 'Games',
    url: '#',
    current: false,
  },
  {
    text: 'Collectibles',
    url: '#',
    current: false,
  },
  {
    text: 'Videos',
    url: '#',
    current: false,
  },
  {
    text: 'Fans',
    url: '#',
    current: false,
  },
  {
    text: 'News',
    url: '#',
    current: false,
  },
  {
    text: 'Shop',
    url: '#',
    current: false,
  },
]


    }
  }
}
</script>

<style scoped>

header{
    height:200px; 
}

.wrapper{
    height: 200px;
    display:flex; 
    justify-content: space-between;
    align-items: center;
}

nav ul{
    display: flex;
    align-items: center;
    height: 200px;
}

nav ul li{
    margin:10px;
    list-style-type: none;
    height: 100%;
    line-height: 200px;
}

nav ul li a {
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    color: darkgray;
    font-size: 0.8rem;
    padding:10px;
    
}

li:hover,
li.active  {
    border-bottom: 5px solid black;
    border-color: #0C7CEC;
    
}






</style>