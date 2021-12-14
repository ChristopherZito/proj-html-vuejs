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
                            <img :src="item.img" alt="">
                        </div>
                        <h2>{{item.title}}</h2>
                        <span>{{item.time}}|
                            <span v-if="item.comments.length != null">{{item.comments.length}} Comments</span>
                            <span v-else>Comments off</span>
                        </span>
                        <p>{{item.text}}</p>
                    </div>
                </div>
            </section>
            <!-- secondo blocco main -->
            <section>
                <!-- title -->
                <!-- text -->
                <!-- button -->
            </section>
            <!-- terzo blocco main -->
            <section>
                <!-- immagini -->
                    <!-- img/title/date/comments/description -->
            </section>
            <!-- quarto blocco -->
            <section>
                <!-- left -->
                <div>
                    <!-- title -->
                    <!-- text -->
                    <!-- button -->
                </div>
                <!-- right -->
                <div>
                    <!-- titolo -->
                    <!-- immagini -->
                    <!-- img/title/date/comments/description -->
                </div>
            </section>
        </section>
       
        <h1 id="break-line">
            READ OUR BLOG 
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

        #up-main {
            h1 {
                font-size: 40px;
            }

            hr {
                width: 100px;
                border: 1px solid #fc8c53;
                margin: 0 auto 50px;
            }
        }

        .box {
            
            display: flex;
            justify-content: space-between;
            
            .none {
                display: none;
            }

            .items{
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;

                width: 30%;
                margin-bottom: 30px;
                text-align: start;
                /* debug */
                /* height: 300px; */
                /* background-color: red;  */  
            }
            

            .img {
                width: 100%;
                /* debug */
                background-color: black;
                height: 200px;

                img{
                    width: 100%;
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
