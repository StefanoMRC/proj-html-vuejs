<template>
  
          <li class="w-50 py-1">
              <a class="text_chiaro" :href="link">{{nome}}</a>
          </li>
     
</template>

<script>
export default {
  name: 'CompLink',
    props:{
        nome:String,
        link:String
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    div{
       
        ul{
            
            li{
                a{
                    text-decoration: none;
                    font-weight: bold;
                }
                a:hover{
                    color: #1fad96;
                }
            }
        }
    }
</style>
