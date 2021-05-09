<template>
   <div class="container">
       <img :src="element.trumb" :alt="element.series">
       <p>{{element.series}}</p>
   </div>
</template>

<script>
export default {
   name: 'Comics',
   props: ['element']
}
</script>

<style>

</style>>

</style>