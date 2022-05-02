<template>
<div class="text_chiaro">
  <ul v-for="(element, index) in indirizzo" :key="index">
      <li class="pt-2">
          {{element.nome}}
      </li>
      <li class="py-2">
          {{`${element.numero}${element.orariApertura}`}}
      </li>
      <li>
          {{element.email}}
      </li>
  </ul>
</div>
  
</template>

<script>
export default {
  name: 'CompIndirizzo',
  props:{
    indirizzo:Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  ul{
    list-style-type: none;
    padding: 0;
    font-weight: bold;
  }
</style>