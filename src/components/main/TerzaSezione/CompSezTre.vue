<template>
  <div class="col-2">
     
          <img class="img-fluid" :src="immagine" alt="">
      
  </div>
</template>

<script>
export default {
  name: 'CompSezTre',
  props:{
      immagine:String
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
