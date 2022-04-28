<template>
      <li class="flex align_center">
          <a :href="link">{{nome}}</a>
      </li> 
</template>

<script>
export default {
  name: 'MenuComp',
  props:{
      'nome':String,
      'link':String

  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    li{
        
        a{
            color: white;
            margin: 0 10px;
        }
    }
</style>