<template>
  <div id="container">
      <section id="middle">
            <!-- primo blocco main -->
            <section id="up-main">
                <!-- titolo -->
                <h4>
                    PHASELLUS EGET METUS
                </h4>
                <h1>
                    All the latest news
                </h1>
                <hr>
                <!-- immagini  img/title/date/comments/description -->
                <div class="box" >
                    <div :class="item.position == `top` ? `items` : `none`" v-for="item,i in products" :key="i">
                        <div class="img">
                            <img :src="require(`@/assets/img/${item.img}`)" :alt="item.title">
                        </div>
                        <h5>{{item.title}}</h5>
                        <span>{{item.time}}|
                            <span v-if="item.comments.length != null">{{item.comments.length}} Comments</span>
                            <span v-else>Comments off</span>
                        </span>
                        <p>{{item.text}}</p>
                    </div>
                </div>
            </section>
            <!-- secondo blocco main -->
            <section id="more-info">
                <!-- title -->
                <h5>FEATURED ARTICLE</h5>
                <h1>Cras malesuada er orci eget pharetra</h1>
                <!-- text -->
                <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum sadips ets ipsums dolores ficilis uns leo lectus.</p>
                <!-- button -->
                <button>READ MORE <i class="fas fa-angle-right"></i> </button> 
            </section>
            <!-- terzo blocco main -->
            <section>
                <div class="box" >
                    <div :class="item.position == `bottom` ? `items` : `none`" v-for="item,i in products" :key="i">
                        <div class="img">
                            <img :src="require(`@/assets/img/${item.img}`)" :alt="item.title">
                        </div>
                        <h5>{{item.title}}</h5>
                        <span>{{item.time}}|
                            <span v-if="item.comments.length != null">{{item.comments.length}} Comments</span>
                            <span v-else>Comments off</span>
                        </span>
                        <p>{{item.text}}</p>
                    </div>
                </div>
            </section>
            <!-- quarto blocco -->
            <section id="lower-main">
                <!-- left -->
                <div id="left-lower">
                    <!-- title -->
                    <h5>REVIEWED PRODUCT</h5>
                    <h1>Mauris viverra atisan ipsum eget felis prims efficitur varius</h1>
                    <!-- text -->
                    <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum.</p>
                    <!-- button -->
                    <button>READ MORE <i class="fas fa-angle-right"></i> </button> 
                </div>
                <!-- right -->
                <div id="right-lower">
                    <!-- titolo -->
                    <h1>Tutorials &amp; guides</h1>
                    <hr>
                    <div class="column" >
                        <div :class="item.tutorial == true ? `tutorial` : `none`" v-for="item,i in products" :key="i">
                            <div class="toImg">
                                <img :src="require(`@/assets/img/${item.img}`)" :alt="item.title">
                            </div>
                            <span>
                                <h5>{{item.title}}</h5>
                                <span>{{item.time}}|
                                    <span v-if="item.comments.length != null">{{item.comments.length}} Comments</span>
                                    <span v-else>Comments off</span>
                                </span>
                            </span>
                        </div>
                    </div>
                </div>
            </section>
        </section>
       
        <h1 id="break-line">
            READ OUR BLOG <i class="fas fa-long-arrow-alt-right"></i>
        </h1>
  </div>
</template>

<script>
export default {
    name: 'News',
    props: {
        products: Array,
    }, 
}
</script>

<style scoped lang="scss">
#container {
    text-align: center;
    #middle {
        width: 60%;
        margin: auto;
        .none {
            display: none;
        }
        #up-main {
            padding: 50px 0;
            h1 {
                font-size: 40px;
                margin: 20px 0;
            }
            hr {
                width: 100px;
                border: 0.5px solid #fc8c53;
                margin: 0 auto 50px;
            }
        }
        .box {
            display: flex;
            justify-content: space-between;
            span {
                font-size: 10px;
                color: #62676c;
                margin: 10px 0 ;
            }
            p {
                color: #62676c;
                font-size: 12px;
                line-height: 20px;
            }
            .items{
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;

                width: 30%;
                /* margin-bottom: 30px; */
                text-align: start;
                /* debug */
                /* height: 300px; */
                /* background-color: red;  */  
            }
            .img {
                width: 100%;
                /* debug */
                /* background-color: black; */
                /* height: 202px; */
                img{
                    width: 100%;
                }
            }
        }
        #more-info {
            background-image: url("../assets/img/featured_article_1_bg.jpg");
            background-position: center;
            background-size: cover;
            text-align: start;
            color: #ffff;
            padding: 200px 70px 100px;
            margin-bottom: 30px;
            /* debug */
            /* height: 400px; */

            h1 {
                font-size: 30px;
                font-weight: 600;
                margin: 20px 0;
            }
            button {
                padding: 10px 30px;
                color: #ffff;
                background-color: black;
                margin-top: 30px;
                border: none;
            }
        }
        #lower-main {
            margin: 50px 0;
            display: flex;
            justify-content: space-between;
            #left-lower {
                width: 65%;
                background-image: url("../assets/img/featured_article_2_bg.jpg");
                background-position: center;
                background-size: cover;
                text-align: start;
                color: #ffff;
                padding: 60px;

                p {
                    font-size: 12px;
                }
                h1 {
                    font-size: 30px;
                    font-weight: 600;
                    margin: 20px 0;
                }
                button {
                    padding: 10px 30px;
                    color: #ffff;
                    background-color: black;
                    margin-top: 30px;
                    border: none;
                }
            }

            #right-lower {
                width: 30%;
                text-align: start;
                hr {
                    width: 100px;
                    border: 0.5px solid #fc8c53;
                    margin: 20px 0;
                }
                .column {
                    display: flex;
                    flex-direction: column;

                    .tutorial {
                        display: flex;
                        .toImg {
                            margin-right: 15px;
                            
                            img {
                                width: 100%;
                            }
                        }
                        span {
                            font-size: 9px;
                            color: #62676c;

                            h5 {
                                color: black;
                                font-size: 11px;
                                font-weight: 800;
                            }
                        }
                    }
                }

            
            }
        }
    }


    #break-line {
        width: 100%;
        color: #ffff;
        background-color: black;
        padding: 50px 0;
    }
}
</style>
