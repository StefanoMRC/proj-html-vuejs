<template>
  <div class="cont_principale">
   <div class="cont_secondario py-5">
       <div class="container">
           <div class="row ">
                <div class="col-6">
                    <h2 class="fw-bold">Address</h2>
                    <CompIndirizzo
                    v-for="(element, index) in listaIndirizzo" :key="index"
                    :indirizzo='listaIndirizzo'
                    />
                    <div>
                        <ul class=" d-flex">
                            <li><a class="text_chiaro" href=""><i class="fa-brands fa-facebook-square fs-4"></i></a></li>
                            <li class="px-4"><a class="text_chiaro " href=""><i class="fa-brands fa-twitter fs-4"></i></a></li>
                            <li><a class="text_chiaro" href=""><i class="fa-brands fa-instagram-square fs-4"></i></a></li>
                            <li class="ps-4"><a class="text_chiaro " href=""><i class="fa-brands fa-linkedin fs-4"></i></a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-3 explore">
                    <h2 class="fw-bold">Explore</h2>
                    <ul class="d-flex flex-column flex-wrap h-100">
                        <CompLink
                    v-for="(element, index) in listaExplore" :key="index"
                    :nome='element.nome'
                    :link='element.link'
                    />
                    </ul>
                    
                </div>
                <div class="col-3">
                    <h2 class="fw-bold">Information</h2>
                    <ul class="d-flex flex-column flex-wrap h-100">
                        <CompLink
                    v-for="(element, index) in listaInformazioni" :key="index"
                    :nome='element.nome'
                    :link='element.link'
                    />
                    </ul>
                </div>  
           </div>
           <div class="pt-5">
               <p class="text-center text_chiaro">
                   <i class="fa-solid fa-copyright"></i> 2020 Maxcoach. <span class="text-capitalize">all right reserved</span>
               </p>
           </div>
       </div>
      
   </div>
  </div>
</template>

<script>
import CompIndirizzo from './CompIndirizzo.vue'
import CompLink from './CompLink.vue'
export default {
  name: 'FooterComp',
  components:{
      CompIndirizzo,
      CompLink
  },
    data() {
        return {
            listaIndirizzo:[
                {
                    nome:'382 NE 191st ST # 87394 Miami, FL 33179-3899',
                    numero:'+1(305) 547-9909',
                    orariApertura:'9am - 5pm EST, Maonday - Fraiday',
                    email:'support@maxcoach.com'
                }
            ],
            listaExplore:[
                {
                    nome:'Start here',
                    link:'starthere/'
                },
                {
                    nome:'Blog',
                    link:'Blog/'
                },
                {
                    nome:'About us',
                    link:'aboutus/'
                },
                {
                    nome:'Success story',
                    link:'successstory/'
                },
                {
                    nome:'Courses',
                    link:'courses/'
                },
                {
                    nome:'Contact us',
                    link:'contact/'
                },
            ],
            listaInformazioni:[
                {
                    nome:'Membership',
                    link:'membership/'
                },
                {
                    nome:'Purchase guide',
                    link:'purchaseguide/'
                },
                {
                    nome:'Privacy policy',
                    link:'privacypolicy/'
                },
                {
                    nome:'Terms of service',
                    link:'termsofservice/'
                },
            ]
        }
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .cont_principale{
        background: #f8f8f8;
        .cont_secondario{
            width: 80%;
            margin: auto;
            
            .explore{
                height: 120px;
                
            }
            ul{
                    list-style-type: none;
                    padding: 0;
                }
            
        }
    }
</style>
