<template>
  <div>
      <SezUno/>
      <SezUnoDue/>
      <SezDue/>
      <SezTre/>
      <SezQuattro/>
  </div>
</template>

<script>
import SezUno from './PrimaSezione/SezUno.vue'
import SezUnoDue from './PrimaSezione/SezUnoDue.vue'
import SezDue from './SecondaSezione/SezDue.vue'
import SezTre from './TerzaSezione/SezTre.vue'
import SezQuattro from './QuartaSezione/SezQuattro'
export default {
  name: 'MainComp',
    components:{
        SezUno,
        SezUnoDue,
        SezDue,
        SezTre,
        SezQuattro
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>