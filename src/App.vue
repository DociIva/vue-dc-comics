<template>
  <div id="app">
     <!--Header-->
       <Header />

     <!--Main-->
     <main>
        <Products />
     </main>

     <!--Footer-->
     <footer>
        <Footer /> 
     </footer>

    <!--puoi cancellare dopo-->
    <!--<img alt="Vue logo" src="./assets/logo.png">-->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Products from '@/components/Products.vue';
import Footer from '@/components/Footer.vue';

//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
      Header,
      Products,
      Footer,
  
    // HelloWorld:HelloWorld come se fosse cosi ma e abbreviato
  }
}
</script>

<style lang="scss">
// qua vanno gli stili per tutta la pagina
// se vuoi poi importali
// general importazione
@import './styles/general.scss';
// utilities importazione
@import './styles/utilities.scss';

</style>
