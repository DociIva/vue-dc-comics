<template>
  <main class="products">
    <div class="cards">
    <Comics v-for="(comic, index) in comics" :key="index" :elements="comic"> </Comics>
    </div>
      
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
    
  },
  methods: {
  
  }
}
</script>

<style scoped lang="scss">
.products {
  color: #fff;
  background: black;
  text-align: center;
} 
.cards {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
</style>