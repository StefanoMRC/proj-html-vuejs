<template>
    <div class="cont_principale pt-5">
        <div class="cont_secondario ">
            <div class="text-center py-5">
                <h6 class="text-uppercase text_chiaro">wanna trasform your live?</h6>
                <h2 class="fs-1">Glad to <span class="text_green text-capitalize">help you</span> Learn</h2>
            </div>
            <div class="container my-5">
                <div class="row">
                    <div v-for="(element, index) in listaServizi" :key="index" class="col-3">
                        <img class="img-fluid" :src="element.img" alt="">
                        <h3 class="py-2 text-capitalize">{{element.titolo}}</h3>
                        <p class="text_chiaro fs-5">{{element.descrizione}}</p>
                    </div>
                </div>
                
            </div>
            <div class="text-center mt-5 pt-5 cont_pallini">
                    <img class="img-fluid service" src="../../../assets/img/home-6-services-image-1024x411.png" alt="">
                    <div class="pallino_big pallino_blu"></div>
                    <div class="pallino_small pallino_orange"></div>
                    <div class="pallino_big pallino_yellow"></div>
                    <div class="pallino_big pallino_lightblu"></div>
                    <div class="pallino_small pallino_red"></div>
                    <div class="pallino_small pallino_azzurro"></div>    
            </div>
        </div>
    </div>
</template>

<script>
    import img from '../../../assets/img/icons8-bandiera-2-100.png'
    import img2 from '../../../assets/img/icons8-ingra100.png'
    import img3 from '../../../assets/img/icons8-salvagente-100.png'
    import img4 from '../../../assets/img/icons8-monitor-100.png'
    export default {
        name: 'QuintaSez',
        data() {
            return {
                listaServizi: [{
                        titolo: 'idea discussion',
                        descrizione: 'Get teamed up with the specialist who work and teach coding for years at famous universities.',
                        img: img

                    },
                    {
                        titolo: 'web development',
                        descrizione: 'Learn to start building a webpage from scratch. You decide your own pace, course and speed.',
                        img: img2

                    },
                    {
                        titolo: 'sistem administration',
                        descrizione: 'Learners are ancouraged to study the mechanism and structure of system administration.',
                        img: img3

                    },
                    {
                        titolo: 'graphic design',
                        descrizione: 'Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.',
                        img: img4

                    }
                ]
            }
        },
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .cont_principale {


        background-image: linear-gradient(to bottom,
        #fcfcfd 0%,
        #eef0f4 30%, 
        #eef0f4 100%);

        .cont_secondario {
            width: 80%;
            margin: auto;
        }
        .cont_pallini{
            position: relative;
            .service{
                margin-bottom: -28px;
            }
            .pallino_blu{
                border: 5px solid #bce6df;
                top: 0;
                left: 18%;
            }
            .pallino_orange{
                background: #fa7d61;
                bottom: 10%;
            }
            .pallino_yellow{
                background: #ebb860;
                bottom: -55%;
                left: 35px;
            }
            .pallino_lightblu{
                background: #bce6df;
                right: 10%;
                top:10%
            }
            .pallino_red{
                background: #e28794;
                right: 18%;
                bottom: -35px;
            }
            .pallino_azzurro{
                background: #aab8f1;
                right: 0;
                bottom: -55%;
            }
        }
    }
</style>