<template>
    <div class="bg_dark_blue ">
        <div class="flex between align_cente cont_header">
            <div><img class="logo" src="../../assets/img/light-logo.png" alt="immagine logo"></div>
            <div class="flex align_center">
                <ul class="flex ">
                    <MenuComp v-for="(element, index) in listaMenu" :key="index" :nome='element.nome'
                        :link='element.link' />
                </ul>
                <img class="carrello" src="../../assets/img/icons8-carrello-della-spesa-24.png" alt="">
                <div class="contatore">0</div>
                <img class="profilo" src="../../assets/img/icons8-utente-uomo-cerchiato-32.png" alt="">
                <div class="cont_input">
                    
                    <input class="ricerca" type="text" placeholder="Search...">
                    <span class="icona"><i class="fa-solid fa-magnifying-glass"></i></span>
                </div>
                
            </div>
        </div>

    </div>
</template>

<script>
    import MenuComp from './MenuComp.vue'
    export default {
        name: 'HeaderComp',
        components: {
            MenuComp
        },
        data() {
            return {
                listaMenu: [{
                        nome: 'Home',
                        link: 'home/'
                    },
                    {
                        nome: 'Pages',
                        link: 'pages/'
                    },
                    {
                        nome: 'Courses',
                        link: 'courses/'
                    },
                    {
                        nome: 'Featuers',
                        link: 'featuers/'
                    },
                    {
                        nome: 'Blog',
                        link: 'blog/'
                    },
                    {
                        nome: 'Shop',
                        link: 'shop/'
                    },
                ]
            }
        },

    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.cont_header{
    width: 70%;
    margin: auto;
    padding: 10px;
    .logo{
        height: 40px;
    }
    ul {
        list-style-type: none;
    }
    .carrello{
        height: 30px;
        width: 30px;
        filter: invert(2);
        
    }
    .contatore{
        background: white;
        height: 13px;
        width: 13px;
        font-size: 10px;
        text-align: center;
        font-weight: bolder;
        border-radius: 50%;
        margin-left: -10px;
        margin-top: -25px;
        line-height: 13px;
        vertical-align: middle;
    }
    .profilo{
        height: 25px;
        width: 25px;
        filter: invert(2);
        margin: 0 20px;
    }
    .cont_input{
        position: relative;
        
        .icona{
            position: absolute;
            right: 6px;
            top: 6px;
            
            i{
                font-size: 25px;
                color: #1fad96;
            }
        
        }
        .ricerca{
            padding-left: 20px;
            padding-right: 33px;
            height: 40px;
            border-radius: 10px;
            font-size: 20px;
        }
        
    }
    
}
    
</style>