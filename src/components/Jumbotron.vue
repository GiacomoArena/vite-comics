
<script>


export default {
  name:'Jumbotron',

  data(){
    return{
      
    }
  }
}
</script>

<template>
  <section>
    
  </section>
</template>

<style lang="scss" scoped>
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;

section{
  width: 100%;
  height: 350px;
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

</style>