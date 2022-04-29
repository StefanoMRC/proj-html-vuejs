<template>
  <div class="cont_principale">
      <div class="cont_secondario py-5">
          <div class="text-center">
                <h6 class="text_chiaro text-uppercase">enjoy reading on maxcoach</h6>
                <h2 class="fs-1">Lasted on <span class="text-capitalize text_green">our blogs</span></h2>
          </div>
          <div class="container">
              <div class="row">
                  <CompSezQuattro
                  v-for="(element, index) in listaArticoli" :key="'A'+index"
                  :descrizione='element.nome'
                  :tipo='element.tipo'
                  :data='element.data'
                  :visualizzazioni='element.views'
                  :immagine='element.img'
                  />
              </div>
          </div>
          
      </div>
  </div>
</template>

<script>
import img from '../../../assets/img/artist-blog-03-480x325.jpeg'
import img1 from '../../../assets/img/artist-blog-01-480x325.jpg'
import img2 from '../../../assets/img/artist-blog-02-480x325.jpg'
import CompSezQuattro from './CompSezQuattro.vue'
export default {
    
  name: 'SezQuattro',
  components:{
        CompSezQuattro
    },
    data() {
        return {
            listaArticoli:[
                {
                    nome:'brush strokes energize trees in paintings',
                    tipo:'artist',
                    data:'May 15, 2020',
                    views:688,
                    img:img
                },
                {
                    nome:'pocket-sized notebooks hold miniature paintings',
                    tipo:'artist',
                    data:'May 15, 2020',
                    views:688,
                    img:img1
                },
                {
                    nome:'connection between self-portraits and identity',
                    tipo:'artist',
                    data:'May 15, 2020',
                    views:688,
                    img:img2
                }
            ]
        }
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .cont_principale{
        
        background: #f5f7fa;
        .cont_secondario{
            width: 80%;
            margin: auto;
        }
    }
</style>