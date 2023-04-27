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
      </li>
      </ul>
    </section>
  </div>
</template>


<style lang="scss" scoped>
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/mixin" as *;
  .container{
    color: $secondary-color;
    display: flex;
  }
</style>