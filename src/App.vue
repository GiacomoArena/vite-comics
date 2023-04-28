  <script>

    import Header from './components/Header.vue';
    import Main from './components/Main.vue';
    import Info from './components/Info.vue';
    import Footer from './components/Footer.vue';
    import Contact from './components/Contact.vue';
    import Jumbotron from './components/Jumbotron.vue';

  export default {
    name:'App',
    components:{
      Main,
      Header,
      Info,
      Footer,
      Contact,
      Jumbotron
    },
    data(){
      return{

      }
    }
  }
  </script>


<template>
  

  <Header />

  <Jumbotron />
  
  <Main />

  <Info />
  
  <Footer />

  <Contact />

</template>


<style lang="scss">
  @use './scss/main.scss';

</style>