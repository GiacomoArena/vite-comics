  <script>
  import {headerMenu} from '../data/db';

  export default {
    name: 'Header',

    data(){
    return{
      headerMenu,
    }
  }
  }
  
  </script>

<template>
  <div class="container">
    <section class="logo">
      <img src="../assets/img/dc-logo.png" alt="logo">
    </section>
    
    <section class="links">
      <ul>
        <li 
        v-for="(link, i) in headerMenu" 
        :key="i">
        <a :href="link.href">
          {{ link.menu }}
          <span>_</span>
        </a>
        
      </li>
      </ul>
    </section>
  </div>
</template>


<style lang="scss" scoped>
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;
  .container{
    height: 100px;
    color: $secondary-color;
    display: flex;
    justify-content: space-between;
    align-items: center;
    img{
      width: 70px;
    }
    ul{
      display: flex;
    }
    a{
      position: relative;
      padding: 15px;
      font-weight: 500;
      color: $secondary-color;
      text-transform: uppercase;
      
    }
    span{
      right: 35%;
      top: 13px;
      height: 0;
      position: absolute;
      color: $primary-color;
      font-size: 60px;
      opacity: 0;
      }
      a:hover{
        color: $primary-color;
      }
      a:hover span{
        opacity: 1;
      }
  }
</style>