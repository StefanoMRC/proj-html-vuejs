<template>
  <div>
      <SezUno/>
      <SezUnoDue/>
      <SezDue/>
  </div>
</template>

<script>
import SezUno from './PrimaSezione/SezUno.vue'
import SezUnoDue from './PrimaSezione/SezUnoDue.vue'
import SezDue from './SecondaSezione/SezDue.vue'
export default {
  name: 'MainComp',
    components:{
        SezUno,
        SezUnoDue,
        SezDue
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>