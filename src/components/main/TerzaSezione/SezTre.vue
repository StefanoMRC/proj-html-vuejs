<template>
    <div class="cont_principale py-5">
        <div class="cont_secondario">
            <h2 class="text-center text-capitalize fs-1 pb-5">
                why peaple talk about <span class="text_green">maxChoach</span>?
            </h2>
            <div class="container mt-5">
                <div class="row align-items-center justify-content-center cont_avatar">
                    <div class="col-3 ">
                        <img class="rounded-circle" src="../../../assets/img/testimonial-avata-02.jpg" alt="">
                        <img class="sfondo_avatar" src="../../../assets/img/maxcoach-shape-05-100x100.png" alt="">
                        <div class="pallino_brown"></div>

                    </div>
                    <div class="col-6">
                        <p class="fs-3">
                            I am free to learn at my own peace, follow my own schedule and choose the subject I like.
                            Great study portal for peaple like me.
                        </p>
                        <h6 class="text-uppercase">mina hollace</h6>
                        <span class="text_chiaro ">/Freelancer</span>
                    </div>

                </div>
                <div class="row mt-5 py-5 justify-content-between align-items-center">
                    <CompSezTre
                    v-for="(element, index) in listaImmagini" :key="index"
                    :immagine='element.img'
                    />
                </div>
            </div>
            
        </div>
    </div>
</template>

<script>
import img1 from '../../../assets/img/client-logo-colored-01.png'
import img2 from '../../../assets/img/client-logo-colored-02.png'
import img3 from '../../../assets/img/client-logo-colored-03.png'
import img4 from '../../../assets/img/client-logo-colored-04.png'
import img5 from '../../../assets/img/client-logo-colored-05.png'
import img6 from '../../../assets/img/client-logo-colored-06.png'
import CompSezTre from './CompSezTre.vue'
    export default {
        name: 'SezTre',
        components:{
            CompSezTre
        },
        data() {
            return {
                listaImmagini:[
                    {
                        img:img1
                    },
                    {
                        img:img2
                    },
                    {
                        img:img3
                    },
                    {
                        img:img4
                    },
                    {
                        img:img5
                    },
                    {
                        img:img6
                    },
                ]
            }
        },
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .cont_principale {
        padding: 30px 0;

        .cont_secondario {
            width: 80%;
            margin: auto;
            .cont_avatar{
                position: relative;
            }
            .sfondo_avatar{
                position: absolute;
                bottom: -38px;
                left: 19%;
                z-index: -1;
                width: 115px;
            }
            .pallino_brown{
                height: 80px;
                width: 80px;
                border-radius: 50%;
                background: #d2a98e;
                position: absolute;
                top: -18px;
                left: 15%;
                z-index: -1;
            }
        }
    }
</style>