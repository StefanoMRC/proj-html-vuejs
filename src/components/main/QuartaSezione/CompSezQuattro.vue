<template>
  <div class="col-4 p-3">
      <img class="img-fluid" :src="immagine" alt="">
      <h6 class="text-uppercase text_chiaro mt-3">{{tipo}}</h6>
      <h2 class="text-capitalize py-2">{{descrizione}}</h2>
      <div>
          <span class="text_chiaro me-3"><i class="fa-solid fa-calendar-week me-2"></i>{{data}}</span>
          <span class="text_chiaro"><i class="fa-solid fa-eye me-2"></i>{{`${visualizzazioni} views`}}</span>
      </div>
  </div>
</template>

<script>
export default {
  name: 'CompSezQuattro',
    props:{
        immagine:String,
        descrizione:String,
        tipo:String,
        visualizzazioni:Number,
        data:String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
