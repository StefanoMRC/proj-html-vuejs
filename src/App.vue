<template>
  <div id="app">
    <HeaderComp/>
    <HeroComp/>
    <MainComp/>
    <FooterComp/>
  </div>
</template>

<script>
import "bootstrap"
import HeaderComp from './components/header/HeaderComp.vue'
import HeroComp from './components/hero/HeroComp.vue'
import MainComp from './components/main/MainComp.vue'
import FooterComp from './components/footer/FooterCom.vue'
export default {
  name: 'App',
  components: {
    HeaderComp,
    HeroComp,
    MainComp,
    FooterComp
  }
}
</script>

<style lang="scss">
  @import "bootstrap/dist/css/bootstrap.min.css";
  @import url('https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@300&family=Lato:ital,wght@1,300&family=Roboto:wght@300&display=swap');
  *{
    font-family: 'Josefin Sans', sans-serif;
    font-family: 'Lato', sans-serif;
    font-family: 'Roboto', sans-serif;
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
  .pallino_big {
        height: 50px;
        width: 50px;
        border-radius: 50%;
        position: absolute;
      }
  .pallino_small {
        height: 30px;
        width: 30px;
        border-radius: 50%;
        position: absolute;
      }    
</style>
