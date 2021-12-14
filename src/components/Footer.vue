<template>
    <div>
        <section id="container">
            <!-- 4 info item -->
            <div class="block" v-for="element,i in info" :key="i">
                <h1>{{element.title}}</h1>
                <p>{{element.text}}</p>
                <ul>
                    <li v-for="refTo, o in element.ref" :key="o">
                        <i class="fas fa-angle-right"></i>
                        {{refTo.text}}
                        <hr>
                    </li>
                </ul> 
            </div>
        </section>
        
        <section id="social">
            <div id="subFooter">
                <!-- copyright -->
                <div>
                    <p>
                        <i class="far fa-copyright"></i>
                        Copyright 2012 - 2020 | Avada Theme by 
                        <strong>Theme Fusion</strong>
                        | All Rights Reserved| powered by
                        <strong> WordPress</strong>
                    </p>
                </div>
                <!-- social -->
                <div id="link">
                    <i class="fab fa-facebook-f"></i>
                    <i class="fab fa-twitter"></i>
                    <i class="fab fa-instagram"></i>
                    <i class="fab fa-youtube"></i>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: 'Footer',
    props: {
        info:Array,
    }
}
</script>

<style scoped lang="scss">

#container {
    width: 60%;
    margin: auto;
    display: flex;
    justify-content: space-between;


    .block {
        width: 22%;
        padding: 60px 0px;
        /* debug */
        /* background-color: blue; */

        p {
            color: grey;
            margin: 20px 0;
            line-height: 25px;
        }

        li {
            list-style: none;
            margin: 20px 0;
            
            hr {
                margin: 10px 0;
                color: #aeaeae;
            }

            i {    
            margin:0 5px 0 -15px;
            }
        }
    }
    
}

#social {
    border-top: 1px solid #aeaeae;

    #subFooter{
        padding: 40px 0;
        width: 60%;
        margin: auto;
        display: flex;
        justify-content: space-between;

        p {
            font-size: 10px;
            color: #898989;
            strong {
                color: #000;
            }
        }

        #link {
            i {
                font-size: 10px;
                padding: 10px 12px;
                color: white;
                border-radius: 50%;
                margin: 0 10px;
            }
            .fa-facebook-f {
                background-color: #4562b0;
            }
            .fa-twitter {
                background-color: #74def4;
            }
            .fa-instagram {
                background-color: #516faa;
            }
            .fa-youtube {
                background-color: #951a0c;
            }
        }  
    }
}

</style>