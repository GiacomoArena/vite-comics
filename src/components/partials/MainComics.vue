
<script>
export default {
  name:'MainComics',
  props:{
    itemThumb: String,
    itemSeries: String
  },
  mounted(){
    console.log(this.itemThumb);
  }
}
</script>


<template>
  <div class="props-container">
      <img :src="itemThumb" alt="">
      <h5>{{ itemSeries }}</h5>
  </div>
</template>

<style lang="scss" scoped>
 @use "../../scss/partials/vars" as *;
  
  .props-container{
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    width: calc(100% /6);
    
    img{
      width: 150px;
      height: 200px;
      margin-bottom: 15px;
      cursor: pointer;
      transition: all 1s;
    }
    img:hover{
      width: 200px;
      height: 250px;
      transform: scale(1);

    }
    h5{
      color: white;
      margin-bottom: 20px;
      text-transform: uppercase;
    }
  }

</style>
