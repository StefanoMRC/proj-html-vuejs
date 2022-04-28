<template>
  <div class="cont_principale">
      <div class="cont_secondario row">
          <div class="row col-6">
              <div class="col-5 mb-4 mx-2">
                  <div class="my-3 card_custom px-3 pt-3" v-for="(element,index) in listaServizi" :key="index">
                      <h2>{{element.nome}}</h2>
                      <p>{{element.descrizione}}</p>
                      <img :src="element.img" alt="">
                  </div>
              </div>
              <div class="col-5  mx-2 mt-5 ">
                  <div class="my-3 card_custom px-3 pt-3" v-for="(element,index) in listaServizi2" :key="index">
                      <h2>{{element.nome}}</h2>
                      <p>{{element.descrizione}}</p>
                      <img :src="element.img" alt="">
                  </div>
              </div>
          </div>
          <div class="row col-6 align-items-center ">
              <div class="w-75 m-auto">
                    <h5 class="text-uppercase">together we can create</h5>
                    <h2 class="text-capitalize size_custom">services we <span class="text_green">can provide</span> for my clients.</h2>
                    <ul class="p-0">
                        <li><i class="fa-solid fa-check"></i>Select & customize courses to your preferences</li>
                        <li><i class="fa-solid fa-check"></i>Change the tutor and make errangements</li>
                        <li><i class="fa-solid fa-check"></i>Paticipate in events to join others</li>
                        <li><i class="fa-solid fa-check"></i>Get the desired certificate delivered at house</li>
                    </ul>
                    <button class="button">Get started for free</button>
              </div>
              

          </div>
      </div>
  </div>
</template>

<script>
import img from '../../../assets/img/home-6-service-image-01.png'
import img2 from '../../../assets/img/home-6-service-image-02.png'
import img3 from '../../../assets/img/home-6-service-image-03.png'
import img4 from '../../../assets/img/home-6-service-image-04.png'

export default {
  name: 'SezUno2',
    data() {
        return {
            listaServizi:[
                {
                    nome:'Gaphic Design',
                    descrizione:'Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.',
                    img:img   
                },
                {
                    nome:'Idea Discussion',
                    descrizione:'Get teamed up with the specialist who work and teach coding for years at famous universities.',
                    img:img2   
                }],
            listaServizi2:[    
                {
                    nome:'Businnes Administration',
                    descrizione:'Learners are ancouraged to study the mechanism and structure of system administration.',
                    img:img3   
                },
                {
                    nome:'Web Development',
                    descrizione:'Learn to start building a webpage from scratc. You decide your own peace, course and speed.',
                    img:img4  
                },
            ]
        }
    },
}
</script>


<style scoped lang="scss">

    .cont_principale{
        padding-top: 150px;
        background-image: url('../../../assets/img/background-pattern-grid-line.png');
        padding-bottom: 50px;
        .cont_secondario{
            width: 80%;
            margin: auto;
            
            .card_custom{
                background: white;
                box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
            }
            .size_custom{
                font-size: 3.5em;
                .text_green{
                    color: #1fad96;
                }
              
            }
            ul{
                
                li{
                    list-style-type: none;
                    i{
                        color: #1fad96;
                        margin-right: 5px;
                    }
                }
                
            }
            .button{
                padding: 10px 20px;
            }

        }
    }
</style>
