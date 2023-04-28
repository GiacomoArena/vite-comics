  <script>
  import dcComics from '../data/dc-comics.json'
  import MainComics from '../components/partials/MainComics.vue'


  export default {
    name: 'Main',
    components:{
      MainComics
    },
    data(){
      return{
        dcComics,
        
      }
    },
  }

  </script>

<template>

<div class="main-container">
  
  <div class="container">
    
    <MainComics 
  v-for="(item, i ) in dcComics"
  :key="i"
  :itemThumb="item.thumb"
  :itemSeries="item.series"
  />

  </div>

</div>

</template>


<style lang="scss" scoped >
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;
.main-container{
  color: $primary-color;
  background-color: $secondary-color;
  min-height: 100px;
  .container{
    display: flex;
    flex-wrap: wrap;
  }
}

</style>