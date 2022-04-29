<template>
  <div id="app">
    <HeaderComp/>
    <HeroComp/>
    <MainComp/>
  </div>
</template>

<script>
import "bootstrap"
import HeaderComp from './components/header/HeaderComp.vue'
import HeroComp from './components/hero/HeroComp.vue'
import MainComp from './components/main/MainComp.vue'
export default {
  name: 'App',
  components: {
    HeaderComp,
    HeroComp,
    MainComp
  }
}
</script>

<style lang="scss">
  @import "bootstrap/dist/css/bootstrap.min.css";
 
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
    border: 0;
  }
  .text_green{
    color: #1fad96;
  }
  .text_chiaro{
    color: rgba(0, 0, 0, 0.473);
  }
</style>
