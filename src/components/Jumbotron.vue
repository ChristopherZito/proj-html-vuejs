<template>
<section>
    <div id="jumbo">
        <!-- jumbotron -->
        <section>
            <!-- titolo -->
            <h1>Tech Forum!</h1>
            <!-- testo -->
            <p>
                Discuss all the latest technology news and trends
            </p>
            <!-- bottone -->
            <button>
                GET AVADA NOW!  <i class="fas fa-angle-right"></i>
            </button>
        </section>
    </div>
    <!-- testo avada -->
    <div id="text">
        <div>
            <h5>
                AVADA FORUM IS THE PLACE TO BE
            </h5>
            <p>
                In quis lectus sed leo elementum faucibus in dapibus dectum. 
                <br>
                Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus.
                <br>
                dolor at, bibendum purus. Donec veicula nec tortor ac finibus
            </p>
        </div>
    </div>
</section>
</template>

<script>
export default {
name: 'Jumbotron',
}
</script>

<style scoped lang="scss">
#jumbo {
    background-image: url("../assets/img/home_slider_bg.jpg");
    /* debug */
    /* height: 600px; */

    section {
        width: 60%;
        margin: auto;
        padding: 200px 0;
        color: #ffff;

        h1 {
            font-size: 120px;
        }

        button {
            background-color: #27aabe;
            padding: 10px 20px;
            color: #fff;
        }

        p {
            margin: 20px 0;
            font-size: 20px;
            font-weight: normal;
        }
    }
}

#text {
    background-color: #e7e7e7;
    background-position: center;

    div {
        width: 60%;
        margin: auto;
        padding: 50px 0;
        text-align: center;

        p {
            line-height: 30px;
            font-size: 20px;
            margin-top: 30px;
            color: grey;
        }
    }
}

</style>