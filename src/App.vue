  <script>

    import Header from './components/Header.vue'
    import Main from './components/Main.vue'
    import Info from './components/Info.vue'
    import Footer from './components/Footer.vue'

  export default {
    name:'App',
    components:{
      Main,
      Header,
      Info,
      Footer
    },
    data(){
      return{

      }
    }
  }
  </script>


<template>
  

  <Header />

  <Main />

  <Info />
  
  <Footer />

</template>


<style lang="scss">
  @use './scss/main.scss';

</style>