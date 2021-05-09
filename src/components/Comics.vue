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
      width: 50%;
      margin-top: 40px;
      margin-bottom: 10px;
   }
   p {
     text-transform: uppercase;
     margin-bottom: 20px ;
   }
}


</style>
