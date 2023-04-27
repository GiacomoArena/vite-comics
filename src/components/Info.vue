  <script>
    import {InfoMenu} from '../data/db';


  export default {
    name: 'Info',
    
    
    data(){
    return{
      InfoMenu,
    }
  },
  methods:{
    getImage(src){
      return new URL(`../assets/img/${src}`, import.meta.url).href
    }
  }

  }
  </script>

<template>
  <section>
    <div class="container">
      <ul>
        <li
        v-for="(link,i) in InfoMenu"
        :key="i"
        ><a :href="link.href"><img :src="getImage(link.src)" alt="">{{ link.menuString }}</a></li>
      </ul>
    </div>
  </section>
</template>


<style lang="scss" scoped>
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;

  section{
    display: flex;
    align-items: center;
    background-color: $primary-color;
    height: 150px;
    .container{
    }
    ul{
      display: flex;  
      justify-content: space-between;
      align-items: center;
    }
    a{
      display: flex;
      align-items: center;
      color:white;
      text-transform: uppercase;
    }
    a:hover{
      color: $secondary-color;
    }
    img{
      width: 50px;
      margin: 15px;
    }
  }

</style>