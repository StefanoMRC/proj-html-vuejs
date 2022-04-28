<template>
  <div id="app">
    <HeaderComp/>
    <HeroComp/>
  </div>
</template>

<script>

import HeaderComp from './components/header/HeaderComp.vue'
import HeroComp from './components/hero/HeroComp.vue'
export default {
  name: 'App',
  components: {
    HeaderComp,
    HeroComp
  }
}
</script>

<style lang="scss">
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  .flex{
    display: flex;
  }
  .between{
    justify-content: space-between;
  }
  .align_center{
    align-items: center;
  }
  .bg_dark_blue{
    background: #1f2154;

  }
  .button{
    background: #1fad96;
    color: white;
    border-radius: 5px;
  }
</style>
