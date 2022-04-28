<template>
  <div>
      <SezUno/>
      <SezUnoDue/>
  </div>
</template>

<script>
import SezUno from './PrimaSezione/SezUno.vue'
import SezUnoDue from './PrimaSezione/SezUnoDue.vue'
export default {
  name: 'MainComp',
    components:{
        SezUno,
        SezUnoDue
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>