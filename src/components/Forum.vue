<template>
  <div id="container">
        
        <section>
            <!-- title -->
            <h4>
                PHASELLUS EGET METUS
            </h4>
            <h1>
                Forum Sections
            </h1>
            <hr>
            <div id="box">
                <!-- blog section x8 -->
                <div class="forum" v-for="element,i in forum" :key="i">
                    <i :class="element.icon"></i>
                    <h2>
                        {{element.text}}
                    </h2>
                </div>
            </div>
        </section>
        <h1 id="break-line">
            GO TO THE FORUM <i class="fas fa-long-arrow-alt-right"></i>
        </h1>
  </div>
</template>

<script>
export default {
    name: 'Forum',
    data() {
        return {
            forum: [
                {
                    icon:"fas fa-file-alt",
                    text:"News & Community",
                },
                {
                    icon:"fab fa-apple",
                    text:"Apple Forum",
                },
                {
                    icon:"fab fa-windows",
                    text:"Microsoft Forum",
                },
                {
                    icon:"fab fa-android",
                    text:"Android Forum",
                },
                {
                    icon:"fas fa-coffee",
                    text:"General Discussion",
                },
                {
                    icon:"fas fa-cubes",
                    text:"Apps & Software",
                },
                {
                    icon:"fas fa-laptop",
                    text:"Gadgets & Stuff",
                },
                {
                    icon:"fas fa-wrench",
                    text:"Tutorial & Guides",
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
#container {
    text-align: center;
    background-color: #e7e7e7;

    #break-line {
        color: #ffff;
        padding: 50px 0;
        background-color: black;
    }

    section {
        width: 60%;
        margin: auto;
        padding: 50px 0;

        h1 {
            font-size: 50px;
            font-weight: 800;
            margin: 30px 0;
        }

        hr {
            width: 100px;
            border: 1px solid #fc8c53;
            margin: 0 auto 50px;
        }

        #box {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;

            .forum {
                width: 22%;
                border-top: 4px #399bc0 solid ;
                padding: 40px 10px 80px;
                background-color: #ffff;
                margin-bottom: 35px;

                i {
                    font-size: 40px;
                    background-color: #fc8c53;
                    color: #ffff;
                    border-radius: 50%;
                    padding: 20px 25px;
                    margin-bottom: 10px;
                }
            }
        }
    }
}
</style>
