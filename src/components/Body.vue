<template>
    <section>
        <header>
            <Header :position="page"/>
        </header>
        <main>
            <Main :product="page[0].productsHome"/>
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
                    productsHome:[
                        {
                            position:"top",
                            tutorial:false,
                            img:"post_feat_img_25-320x202.jpg",
                            title:"Morbi vitae deu euismod vulptate sollicitudin",
                            time:"October 11th, 2015",
                            text:"Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl",
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
                            img:"post_feat_img_24-320x202.jpg",
                            title:"Vivamus pellenteque, felis quis varius",
                            time:"October 11th, 2015",
                            text:"Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl",
                            comments:{
                            },
                        },
                        {
                            position:"top",
                            tutorial:true,
                            img:"post_feat_img_23-320x202.jpg",
                            title:"Donec ornare pretium eget scelisque justo",
                            time:"October 11th, 2015",
                            text:"Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl",
                            comments:{
                            },
                        },
                        {
                            position:"bottom",
                            tutorial:true,
                            img:"post_feat_img_22-320x202.jpg",
                            title:"Fusce sollicitudin nunc sed placerat varius",
                            time:"October 11th, 2015",
                            text:"Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl",
                            comments:{
                            },
                        },
                        {
                            position:"bottom",
                            tutorial:false,
                            img:"post_feat_img_21-320x202.jpg",
                            title:"Donec facilis sodales leo sit amet laoreet",
                            time:"October 11th, 2015",
                            text:"Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl",
                            comments:{
                            },
                        },
                        {
                            position:"bottom",
                            tutorial:true,
                            img:"post_feat_img_20-320x202.jpg",
                            title:"Proin eu purus sed aru aliquet curabir vens",
                            time:"October 11th, 2015",
                            text:"Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl",
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