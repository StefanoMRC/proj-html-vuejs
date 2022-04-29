<template>
  <div class="cont_principale">
      <div class="cont_secondario">
          <div class="cont_titolo text-center mb-5">
                <h5 class="text-uppercase">choose a course to get started</h5>
                <h2 class="text-capitalize size_custom">lasted featured <span class="text_green">courses</span> </h2>

          </div>
          <div class="row">
              <div v-for="(element, index) in listinoPrezzi" :key="index" class="col-6 d-flex align-items-center cont_card mb-4 p-3">
                  <div class="col-3" >
                      <img class="img-fluid immagine align-self-center" :src="element.img" alt="">
                  </div>
                  <div class="col-9">
                        <h2 v-if="element.prezzo!=0" class="text_green">{{`$${element.prezzo}`}}<span >.00</span></h2>
                        <h2 v-else class="text_green">Free</h2>
                        <h2 class="fs-1">{{element.nome}}</h2>
                        <div class="text_chiaro">
                          <span><i class="fa-solid fa-file-excel me-3"></i>{{element.lezioni}}Lessons</span>
                          <span><i class="fa-solid fa-user mx-3"></i>{{element.studenti}}Students</span>
                        </div>
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
import img1 from '../../../assets/img/sez2img1.jpg'
import img2 from '../../../assets/img/sez2img2.jpg'
import img3 from '../../../assets/img/sez2img3.jpg'
import img4 from '../../../assets/img/sez2img4.jpg'
import img5 from '../../../assets/img/sez2img5.jpg'
import img6 from '../../../assets/img/sez2img6.jpg'
export default {

      name: 'SezDue',
    data() {
        return {
            listinoPrezzi:[
                {
                    nome:'Learning to Write as a Professional Author',
                    prezzo:40,
                    lezioni:20,
                    studenti:50,
                    img:img1
                },
                {
                    nome:'Customer-centric Info-Tech Strategies',
                    prezzo:0,
                    lezioni:24,
                    studenti:769,
                    img:img2
                },
                {
                    nome:'Open Programming Courses for Everyone: Python',
                    prezzo:19,
                    lezioni:17,
                    studenti:62,
                    img:img3
                },
                {
                    nome:'Academic Listening and Note-taking',
                    prezzo:26,
                    lezioni:14,
                    studenti:67,
                    img:img4
                },
                {
                    nome:'Master jQuery in a Short Period of Time',
                    prezzo:39,
                    lezioni:6,
                    studenti:51,
                    img:img5
                },
                {
                    nome:'Introduction to Javascript for Beginners',
                    prezzo:59,
                    lezioni:14,
                    studenti:76,
                    img:img6
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
            padding-top: 50px;
            .cont_titolo{
                h5{
                color: rgba(0, 0, 0, 0.514);
                }
                h2{
                    font-size: 3em;
                    .text_green{
                        color:#1fad96;
                    }
                }
            }
            .immagine{
                height: 170px;
                width: 170px;
                border-radius: 50%;
                filter: saturate(80%);
            }
            .cont_card:hover{
                background: white;
                box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
                h2{
                    color: #1fad96;
                }
                cursor: pointer;
            }
        }
    }
</style>
