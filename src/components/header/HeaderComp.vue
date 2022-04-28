<template>
    <div class="bg_dark_blue ">
        <div class="flex between align_cente cont_header">
            <div><img src="../../assets/img/light-logo.png" alt="immagine logo"></div>
            <div class="flex align_cente">
                <ul class="flex ">
                    <MenuComp v-for="(element, index) in listaMenu" :key="index" :nome='element.nome'
                        :link='element.link' />
                </ul>

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
    width: 80%;
    margin: auto;
    padding: 10px;
    ul {
        list-style-type: none;
    }
}
    
</style>