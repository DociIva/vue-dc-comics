<template>
   <div class="content">
       <img :src="elements.thumb" :alt="elements.series">
       <p>{{elements.series}}</p> 
   </div>
</template>

<script>
export default {
   name: 'Comics',
   props: ['elements']
   
}
</script>

<style scoped lang="scss">
.content {
   flex-basis: calc(100% / 6);
    img {
      width: 40%;
      margin-top: 40px;
      margin-bottom: 10px;
   }
   p {
     text-transform: uppercase;
   }
}


</style>
