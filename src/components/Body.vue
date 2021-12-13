<template>
    <section>
        <header>
            <Header :position="page"/>
        </header>
        <main>
            <Main/>
        </main>
        <footer>
            <Footer/>
        </footer>
    </section>
</template>

<script>
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'
import Footer from '@/components/Footer.vue'

export default {
    name: 'Body',
    components: {
        Header,
        Main,
        Footer
    },
    data() {
        return {
            page: [
                {
                    title:"Home",
                    //prodotti in pagina
                    product:{
                        position:"top",
                        tutorial:false,
                        img:"",
                        title:"",
                        time:"",
                        text:"",
                        comments:{
                            comment:"",
                            comment:"",
                        },
                    },
                    product:{
                        position:"top",
                        tutorial:false,
                        img:"",
                        title:"",
                        time:"",
                        text:"",
                        comments:{
                            comment:"",
                            comment:"",
                        },
                    },
                    product:{
                        position:"top",
                        tutorial:true,
                        img:"",
                        title:"",
                        time:"",
                        text:"",
                        comments:{
                            comment:"",
                            comment:"",
                        },
                    },
                    product:{
                        position:"bottom",
                        tutorial:true,
                        img:"",
                        title:"",
                        time:"",
                        text:"",
                        comments:{
                            comment:"",
                            comment:"",
                        },
                    },
                    product:{
                        position:"bottom",
                        tutorial:false,
                        img:"",
                        title:"",
                        time:"",
                        text:"",
                        comments:{
                            comment:"",
                            comment:"",
                        },
                    },
                    product:{
                        position:"bottom",
                        tutorial:true,
                        img:"",
                        title:"",
                        time:"",
                        text:"",
                        comments:{
                            comment:"",
                            comment:"",
                        },
                    },
                },
                {
                    title:"Apple"
                },
                {
                    title:"Microsoft"
                },
                {
                    title:"Android"
                },
                {
                    title:"Forum"
                },
                {
                    title:"Contact us"
                },
            ],
        }
    }
}
</script>

<style scoped lang="scss">

</style>