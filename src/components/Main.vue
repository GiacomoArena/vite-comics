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
  <span>
    <h4>current series</h4>
  </span>
  <div class="container">
    
    <MainComics 
  v-for="(item, i ) in dcComics"
  :key="i"
  :itemThumb="item.thumb"
  :itemSeries="item.series"
  />

  </div>
  <span>
    <h5>load more</h5>
  </span>
</div>

</template>


<style lang="scss" scoped >
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;
.main-container{
  position: relative;
  color: $primary-color;
  background-color: $secondary-color;
  min-height: 100px;
  padding: 70px 0;
  .container{
    display: flex;
    flex-wrap: wrap;
  }
  span{
    cursor: pointer;
  }
  h4{
    position: absolute;
    top: -25px;
    left: 160px;
    padding: 15px 30px;
    color: white;
    background-color: $primary-color;
    text-transform: uppercase;
    font-size: 1.2rem;
  }
  h5{
    position: absolute;
    bottom: 10px;
    transform: translateX(-50%);
    left: 50%;
    padding: 15px 30px;
    color: white;
    background-color: $primary-color;
    text-transform: uppercase;
    transition: all 1s;
  }
  h5:hover{
    padding: 15px 60px;
  }
}

</style>