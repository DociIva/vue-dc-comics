<template>
  <main class="products">
  
    <Comics v-for="(comic, index) in comics" :key="index" :element="comic"/>
   
      
  </main>
</template>

<script>
import Comics from '@/components/Comics.vue';
import dcComics from '@/data/dcComics.js';
export default {
    name:'Products',
    components: {
      Comics,
    },

   data() {
    return {
      comics: dcComics
    }
  },
  created() {
    //this.getElementCard();
  },
  methods: {
   // getElementCard() {
      // axios.get(dc-comics.js);
    // }
  }
}
</script>

<style scoped lang="scss">
.products {
  height: 200px;
  color: #fff;
  background: black;
  text-align: center;
}


</style>