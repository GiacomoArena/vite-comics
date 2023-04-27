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
        <a :href="link.href">{{ link.menu }}</a>
        <!-- <span>_</span> -->
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
    height: 150px;
    color: $secondary-color;
    display: flex;
    justify-content: space-between;
    align-items: center;
    ul{
      display: flex;
    }
    li{
      position: relative;
    }
    a{
      padding: 15px;
      font-weight: 600;
      color: $secondary-color;
      text-transform: uppercase;
      
    }
    /*span{
      right: 35%;
      top: 41px;
      position: absolute;
      color: $primary-color;
      font-size: 50px;
      opacity: 0;
      }*/
      a:hover{
        color: $primary-color;
      }
      li:hover span{
        opacity: 1;
      }
  }
</style>