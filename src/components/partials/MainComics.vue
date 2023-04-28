
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
      margin-bottom: 15px;
    }
    h5{
      color: white;
    }
  }

</style>
