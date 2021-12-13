<template>
    <section>
        <header>
            <Header :position="page"/>
        </header>
        <main>
            <Main/>
        </main>
        <footer>
            <Footer :info="footer"/>
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
                    products:[
                        {
                            position:"top",
                            tutorial:false,
                            img:"",
                            title:"",
                            time:"",
                            text:"",
                            comments:[
                                {
                                    comment:"",
                                },
                                {
                                    comment:"",
                                },
                            ],
                        },
                        {
                            position:"top",
                            tutorial:false,
                            img:"",
                            title:"",
                            time:"",
                            text:"",
                            comments:{
                            },
                        },
                        {
                            position:"top",
                            tutorial:true,
                            img:"",
                            title:"",
                            time:"",
                            text:"",
                            comments:{
                            },
                        },
                        {
                            position:"bottom",
                            tutorial:true,
                            img:"",
                            title:"",
                            time:"",
                            text:"",
                            comments:{
                            },
                        },
                        {
                            position:"bottom",
                            tutorial:false,
                            img:"",
                            title:"",
                            time:"",
                            text:"",
                            comments:{
                            },
                        },
                        {
                            position:"bottom",
                            tutorial:true,
                            img:"",
                            title:"",
                            time:"",
                            text:"",
                            comments:{
                            },
                        },
                        
                    ],
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
            footer:[
                {
                    title:"AVADA TECH FORUM",
                    text:"Sed semper, nisl id feugiat eleifend, erat est digssim felis, quis auctor elit enim nec ante. Cras et nibh risus. Pellentesque non mi sit amet mi internemtum",
                },
                {
                    title:"POPULAR TOPICS",
                    ref:[
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                    ]
                },
                {
                    title:"RECENT TOPICS",
                    ref:[
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                    ]
                },
                {
                    title:"LATEST REPLIES",
                    ref:[
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                        {
                           text:"Nam a dolor volupat massa auctor semper",
                        },
                    ]
                },
            ],
        }
    }
}
</script>

<style scoped lang="scss">
@import '~@fortawesome/fontawesome-free/css/all.min.css';

header {
    background-color: #27aabe;
    width: 100%;
    /* debug */
    /* height: 100px; */
}
footer {
    width: 100%;
    /* debug */
    /*background-color: red; */
}

</style>