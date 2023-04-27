  <script>
  export default {
    name: 'Footer'
  }
  </script>

<template>
<section>

  <div class="container">
    <div class="lista">
      <ul>
        <li>
          <a href="">ciao</a>
        </li>
      </ul>

      <div class="logo">
        <img src="../assets/img/dc-logo-bg.png" alt="logo">
      </div>
    </div>
    
    
    
    
  </div>

</section>
  
</template>


<style lang="scss" scoped>
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;
  section{
    height: 350px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    .container{
      position: relative;
      display: flex;
      justify-items:flex-end;
      width: 100%;
      height: 100%;
    }
    .lista{
      display: flex;
      justify-content: space-between;
    }
    img{
      right: 15px;
      position: absolute;
      width: 437px;
      height: 350px;
      object-fit: cover;
    }
  }

</style>