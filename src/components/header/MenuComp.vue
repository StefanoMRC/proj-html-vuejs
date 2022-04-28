<template>
      <li>
          <a :href="link">{{nome}}</a>
          <i class="fa-solid fa-angle-down"></i>
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
         margin: 0 10px;
         
        a{
            color: white;
            margin-right: 5px;
            text-decoration: none;
        }
        i{
            color: white;
            font-size: 13px;
        }
    }
</style>