  <script>
    import {dcComics,shop,dc,sites} from '../data/db';


  export default {
    name: 'Footer',
    data(){
    return{
      dcComics,
      shop,
      dc,
      sites
    }
  }
  }
  </script>

<template>
<section>
<!-- ciclare gli li con i valori all intterno del db cosí che sia tutto stampato dinamicamente -->
  <div class="container">
    <div class="lista">
      <ul>
        <h4>dc comics</h4>
        <li
        v-for="(item, i) in dcComics"
        :key="i"
        ><a href="#">{{ item.text }}</a>
        </li>
      </ul> 
      <!-- altra lista -->
      <ul>
        <h4>shop</h4>
        <li
        v-for="(item, i) in shop"
        :key="i"
        ><a href="#">{{ item.text }}</a>
        </li>
      </ul> 
    </div>
    
    
    
    
    <div class="lista">
      <ul>
        <h4>dc</h4>
        <li
        v-for="(item, i) in dc"
        :key="i"
        ><a href="#">{{ item.text }}</a>
        </li>
      </ul> 
    </div>

    <div class="lista">
      <ul>
        <h4>sites</h4>
        <li
        v-for="(item, i) in sites"
        :key="i"
        ><a href="#">{{ item.text }}</a>
        </li>
      </ul> 
    </div>
    
    <img src="../assets/img/dc-logo-bg.png" alt="logo">
    
    
  </div>

</section>
  
</template>


<style lang="scss" scoped>
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;
  section{
    height: 350px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    .container{
      position: relative;
      display: flex;
      justify-items:flex-end;
      width: 100%;
      height: 100%;
    }
    h4{
      text-transform: uppercase;
      color: white;
      margin: 15px 0;
      font-size: 1.5rem;
      cursor: pointer;
    }
    .lista{
      text-transform: capitalize;
      margin: 20px;
      display: flex;
      flex-direction: column;
    }
    a{
      color: rgb(112, 110, 110);
    }
    a:hover{
      color: rgb(255, 255, 255);
    }
    img{
      right: 15px;
      position: absolute;
      width: 437px;
      height: 350px;
      object-fit: cover;
    }
  }

</style>