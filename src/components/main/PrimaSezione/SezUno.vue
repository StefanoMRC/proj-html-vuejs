<template>
  <div class="cont-principale" >
    <div class="cont-secondario text-center" >
      <p class="fs-1 w-50 m-auto">
        Let passion and determination be the guide along the way and develop at your own pace that's comfortable.
      </p>
      <h4 class="text-uppercase pt-4">fannie moreno</h4>
      <span class="color_chiaro">/Founder & CEO</span>
      <div class="pallino_big p_green"></div>
      <div class="pallino_small p_orange"></div>
      <div class="pallino_big p_yellow"></div>
      <div class="pallino_small p_purple"></div>
      <div class="pallino_small p_blu"></div>
      <div class="pallino_small p_red"></div>
      <div class="pallino_small p_light_green"></div>
      <div class="pallino_big p_light_orange"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SezUno',
  data() {
    return {
      listaDati:[
        {
          numeri:1.926,
          descrizione:'finisched sessions'
        },
        {
          numeri:3.092,
          descrizione:'enrolled learners'
        },
        {
          numeri:200,
          descrizione:'online instructors'
        },
        {
          numeri:'100%',
          descrizione:'satisfaction rate'
        },
      ]
    }
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .cont-principale{
    padding-top: 150px;
    .cont-secondario{
      width: 80%;
      margin: auto;
      padding-top: 150px;
      position: relative;
      .color_chiaro{
        color: rgba(0, 0, 0, 0.527);
      }
      .pallino_big{
        height: 50px;
        width: 50px;
        border-radius: 50%;
        position: absolute;
      }
      .pallino_small{
        height: 30px;
        width: 30px;
        border-radius: 50%;
        position: absolute;
      }
      .p_green{
        border: 6px solid #1fad95b9;
        top: 0;
        left: 90px;
      }
      .p_orange{
        background: #e25a6cd2;
        top: 50%;
        left:150px;
      }
      .p_yellow{
        background: #e2a957;
        bottom: 0;
        left: 10px;
      }
      .p_purple{
        background: rgba(128, 0, 128, 0.582);
        left: 40%;
        top:50px;
      }
      .p_light_green{
        background: rgba(32, 178, 171, 0.534);
        top: -65px;
        right: 210px;
        z-index: -1;
      }
      .p_red{
        background: #e25a6cd2;
        top: 40%;
        right: 200px;
      }
      .p_blu{
        background: #1f9ffb7c;
        top: 70%;
        right: 350px;
      }
      .p_light_orange{
        border: 6px solid #e25a6c65;
        bottom: 0;
        right: 200px;
      }
    }
  }
</style>