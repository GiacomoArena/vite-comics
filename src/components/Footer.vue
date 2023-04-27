  <script>
    import {titles} from '../data/db';
    
  export default {
    name: 'Footer',
    data(){
    return{
      titles,
    }
  }
  }
  </script>

<template>
<section>

  <div class="container">
    <div class="lista">
      <ul>
        <h4>dc comics</h4>
        <li>
          <a href="#">characters</a>
        </li>
        <li>
          <a href="#">comics</a>
        </li>
        <li>
          <a href="#">movies</a>
        </li>
        <li>
          <a href="#">TV</a>
        </li>
        <li>
          <a href="#">games</a>
        </li>
        <li>
          <a href="#">videos</a>
        </li>
        <li>
          <a href="#">news</a>
        </li>
      </ul> 
      <!-- altra lista -->
      <ul>
        <h4>shop</h4>
        <li><a href="#">shop DC</a></li>
        <li><a href="#">shop DC collectibles</a></li>
      </ul> 
    </div>
    
    
    
    
    <div class="lista">
      <ul>
        <h4>dc</h4>
        <li><a href="#">terms of use</a></li>
        <li><a href="#">privacy policy(new)</a></li>
        <li><a href="#">ad choices</a></li>
        <li><a href="#">advertising</a></li>
        <li><a href="#">jobs</a></li>
        <li><a href="#">subscriptions</a></li>
        <li><a href="#">talent workshops</a></li>
        <li><a href="#">CPSC certificates</a></li>
        <li><a href="#">rating</a></li>
        <li><a href="#">shop Help</a></li>
        <li><a href="#">contact us</a></li>
      </ul> 
    </div>

    <div class="lista">
      <ul>
        <h4>sites</h4>
        <li><a href="#">DC</a></li>
        <li><a href="#">MAD magazine</a></li>
        <li><a href="#">dc kids</a></li>
        <li><a href="#">dc universe</a></li>
        <li><a href="#">dc power visa</a></li>
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