<template>
  <main class="products">
     <div class="bottone">
       <button>CURRENT SERIES</button>
     </div>
    <div class="cards container">
    <Comics v-for="(comic, index) in comics" :key="index" :elements="comic"> </Comics>
    </div>
    <div class="bottone-s">
      <button>LEAD MORE</button>
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
  position: relative;
} 
.cards {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
.bottone {
  position: absolute;
  top: -30px;
  left: 150px;
}
.bottone button {
  width: 200px;
  height: 60px;
  font-size: 1rem;
  background:#0282f9;
  color:#fff;
  border: 1px solid #000;
  cursor: pointer;
  transition: background 2s;
}
.bottone-s button {
  width: 250px;
  height: 50px;
  margin-bottom: 20px;
  font-size: 1rem;
  background:#0282f9;
  color:#fff;
  border: 1px solid #000;
  cursor: pointer;
  transition: background 2s;
}
button:hover {
  background:limegreen;
}

</style>