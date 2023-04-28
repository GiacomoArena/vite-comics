  <script>


  export default {
    name: 'Contact',
    data(){
    return{
      
    }
  }
  }
  </script>

<template>
  <section>

    <div class="container">
      <div class="sign-up">
        <span>SIGN-UP NOW!</span>
      </div>
  
      <div class="social">
        <h4>FOLLOW US</h4>
        <img src="../assets/img/footer-facebook.png" alt="logo">
        <img src="../assets/img/footer-twitter.png" alt="logo">
        <img src="../assets/img/footer-youtube.png" alt="logo">
        <img src="../assets/img/footer-pinterest.png" alt="logo">
        <img src="../assets/img/footer-periscope.png" alt="logo">
      </div>
    </div>

  </section>
  
</template>


<style lang="scss" scoped>
  @use "../scss/partials/vars" as *;
  @use "../scss/partials/general" as *;
  @use "../scss/partials/mixin" as *;

  section{
    height: 130px;
    display: flex;
    background-color: $footer-color;
  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
    span{
      cursor: pointer;
      color: white;
      font-size:1.2rem ;
      padding: 10px;
      border: 5px solid $primary-color;
    }
    .social{
      display: flex;
      align-items: center;
    }
    img{
      cursor: pointer;
      margin-left: 15px;
      transition: all 1s;
    }
    img:hover{
      width: 50px;
    }
    h4{
      color: $primary-color;
      cursor: pointer;
    }
  }
  
</style>