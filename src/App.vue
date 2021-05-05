<template>
  <div id="app">
     <!--Header-->
       <Header />

     <!--Main-->
     <main>
         <Products/>
     </main>

     <!--Footer-->
     <footer>qua footer</footer>

    <!--puoi cancellare dopo-->
    <!--<img alt="Vue logo" src="./assets/logo.png">-->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Products from '@/components/Products.vue';

//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
      Header,
      Products,
    // HelloWorld:HelloWorld come se fosse cosi ma e abbreviato
  }
}
</script>

<style lang="scss">


/* puoi cancellare dopo
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}*/
</style>
