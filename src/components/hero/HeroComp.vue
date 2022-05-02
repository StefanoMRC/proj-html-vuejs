<template>
  <div class="bg_dark_blue cont_principale">
     <img class="wave" src="../../assets/img/wave.svg" alt="">
     <img class="wave2" src="../../assets/img/wave3.svg" alt="">
 

    <div class="cont_hero">
        <div class="cont_contenuto">
            <h2>learn at your own peace!</h2>
            <p>Get teamed up with peaple of the same will.</p>
            <button class="button" type="button">Get started for free</button>
            <div class="cont_img">
                <div class="hero1">
                    
                </div>
                <div class="hero2 d-flex align-items-center justify-content-center">
                  <img class="youtube" src="../../assets/img/icon-youtube-play.png" alt="">
                </div>
                <div class="hero3">

                </div>
               
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroComp',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .cont_principale{
      position: relative;
      .wave{
            position: absolute;
            bottom: 0;
            z-index: 1;}
      .wave2{
        position: absolute;
        bottom: 0;
        z-index: 0;
      }
      
    }
    .cont_hero{
      width: 80%;
      margin: auto;
      padding-top: 30px;
      
      .cont_contenuto{
        text-align: center;
        color: white;
        
        
        h2{
          font-size: 3em;
          text-transform: capitalize;
        }
        p{
          padding: 20px 0;
        }
        .button{
          padding: 10px 20px; 
        }
        .button:hover{
          background: white;
          color: #1fad96;
        }
        .cont_img{
          display: flex;
          margin-top: 40px;
          justify-content: center;
          
          
          }
          .hero1{
            flex-basis: 30%;
            height: 470px;
            background-image: url('../../assets/img/home-6-hero-left-person-244x300.png');
            background-repeat: no-repeat;
            background-size: contain;
            background-position-x: right;
            background-position-y: bottom;
            align-self: flex-end;
            margin-bottom: -100px;
            margin-right: -10px;
            z-index: 2;
          }
          .hero2{
            flex-basis: 55%;
            align-self: flex-end;
            height: 450px;
            background-image: url('../../assets/img/home-6-hero-poster-final.jpg');
            background-repeat: no-repeat;
            background-position: center;
            z-index: 2;
            background-size: cover;
            border: 20px solid white;
            border-radius: 20px;
            margin-left: -30px;
            margin-bottom: -100px;
            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
            .youtube{
              height: 50px;
            }
          }
          .hero3{
            flex-basis: 25%;
            height: 165px;
            background-image: url('../../assets/img/home-6-hero-right-person-195x300.png');
            background-repeat: no-repeat;
            align-self: flex-end;
            margin-bottom: -100px;
            z-index: 2;
          }

        }
      }
    
  
</style>
