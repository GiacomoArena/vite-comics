
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
  <div>
    <img :src="itemThumb" alt="">
    <h5>ciao</h5>
  </div>
</template>

<style lang="scss" scoped>
 @use "../../scss/partials/vars" as *;
  
  div{
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    width: calc(100% /6);
    img{
      width: 100px;
    }
  }

</style>
