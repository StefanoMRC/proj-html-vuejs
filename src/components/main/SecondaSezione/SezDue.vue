<template>
  <div class="cont_principale">
      <div class="cont_secondario">
          <div class="cont_titolo text-center">
                <h5 class="text-uppercase">choose a course to get started</h5>
                <h2 class="text-capitalize size_custom">lasted featured <span class="text_green">courses</span> </h2>

          </div>
          <div>

          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'SezDue',
    data() {
        return {
            listinoPrezzi:[
                {
                    nome:'Learning to Write as a Professional Author',
                    prezzo:40,
                    lezioni:20,
                    studenti:50
                },
                {
                    nome:'Customer-centric Info-Tech Strategies',
                    prezzo:0,
                    lezioni:24,
                    studenti:769
                },
                {
                    nome:'Open Programming Courses for Everyone: Python',
                    prezzo:19,
                    lezioni:17,
                    studenti:62
                },
                {
                    nome:'Academic Listening and Note-taking',
                    prezzo:26,
                    lezioni:14,
                    studenti:67
                },
                {
                    nome:'Master jQuery in a Short Period of Time',
                    prezzo:39,
                    lezioni:6,
                    studenti:51
                },
                {
                    nome:'Introduction to Javascript for Beginners',
                    prezzo:59,
                    lezioni:14,
                    studenti:76
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
            
        }
    }
</style>
