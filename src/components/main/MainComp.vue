<template>
  <div>
      <SezUno/>
      <SezUnoDue/>
      <SezDue/>
      <SezTre/>
      <SezQuattro/>
      <QuintaSez/>
      <SestSez/>
  </div>
</template>

<script>
import SezUno from './PrimaSezione/SezUno.vue'
import SezUnoDue from './PrimaSezione/SezUnoDue.vue'
import SezDue from './SecondaSezione/SezDue.vue'
import SezTre from './TerzaSezione/SezTre.vue'
import SezQuattro from './QuartaSezione/SezQuattro'
import QuintaSez from './QuintaSezione/QuintaSez.vue'
import SestSez from './SestaSezione/SestaSez.vue'
export default {
  name: 'MainComp',
    components:{
        SezUno,
        SezUnoDue,
        SezDue,
        SezTre,
        SezQuattro,
        QuintaSez,
        SestSez
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>