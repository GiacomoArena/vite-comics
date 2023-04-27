  <script>




  export default {
    name: 'Main',
    
    data(){
    return{
    }
  }
  }
  </script>

<template>

<div class="main-container">
  <h1>/------MAIN-------/</h1>
</div>

</template>


<style lang="scss" scoped >
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;
.main-container{
  text-align: center;
  color: $primary-color;
  background-color: $secondary-color;
  height: 100px;
}

</style>