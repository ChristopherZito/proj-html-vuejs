<template>
    <div id="container">
            <h1>
                GO TO OUR FORUM 
            </h1>
            <section>
                <div id="box">
                     <!-- title -->
                    <h1>
                        Hey! join to our
                        Community
                    </h1>
                    <!-- text -->
                    <p>
                        Nulla molestie tortor nec lectus venenatis, sed blandit deu finibus. Curabitur feugia vulputate purus ipsums dolores ficilis uns etra.
                    </p>
                    <!-- button -->
                    <button>
                        SING UP <i class="fas fa-angle-right"></i>
                    </button>
                </div>
            </section>
    </div>
</template>

<script>
export default {
  name: 'Forum',
}
</script>

<style scoped lang="scss">
#container {
    text-align: center;
    background-color: black;
    color: #ffff;

    h1 {
        padding: 50px 0;
    }

    section {
        background-image: url("../assets/img/join_now_cta_bg.jpg");
        width: 100%;
        /* height: 400px; */

        #box {
            width: 30%;
            margin: auto;
            padding: 140px 0;
        }

        h1 {
            font-size: 50px;
            padding: 0;
        }

        p {
            margin: 20px 0;
            line-height: 40px;
        }

        button {
            font-weight: 600;
            color: #ffff;
            padding: 10px 30px;
            background-color: #2295af;
        }
    }
}

</style>
