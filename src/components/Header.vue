<template>
    <div id="container">
        <!--header -->
        <section>
            <!-- logo -->
            <div id="img">
                <img src="@/assets/img/logo.png" alt="">
            </div>
            <!-- lista info -->
            <span id="box">
                <ul>
                    <li v-for="element, i in position" :key="i">
                        {{element.title}}
                    </li>
                    <li>
                        <!-- bottone -->
                        <button>
                            Join US
                        </button>
                    </li>
                </ul>
                <!-- search -->
                <i class="fas fa-search"></i>
            </span>
        </section>
    </div>
</template>

<script>
export default {
    name: 'Header',
    props: {
        position: Array,
    }
}
</script>

<style scoped lang="scss">
#container {
    width: 60%;
    margin: auto;
    padding: 20px 0;
    color: #ffff;
    /* debug */
    /* background-color: red; */


    section {
        display: flex;
        align-items: center;
        justify-content: space-between;

        #img {
            width: 20%;

            img {
                width: 100%;
            }
        }

        #box{
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 80%;
            ul {
                width: 100%;
                li {
                    margin: 0 20px;
                    display: inline-block;
                }
            }
            
            button
            {
                color: #ffff;
                background-color: black;
                padding: 10px 20px;
            }
        }

    }
}
</style>