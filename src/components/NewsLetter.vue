<template>
  <div>
        <section>
            <!-- title -->
            <h1>
                Subscribe to our Newsletter
            </h1>
            <!-- text area -->
            <input type="text" v-model="text" placeholder="Insert your email*">
            <!-- button -->
            <button @click="sendMail">
                SEND
            </button>
        </section>
  </div>
</template>

<script>
export default {
    name: 'NewsLetter',
    data() {
        return {
            text:"",
        }
    },
    methods: {
        sendMail(){
            this.text = "";
        }
    }
}
</script>

<style scoped lang="scss">
div {
    background-color: #e7e7e7;
    
    section {
        width: 60%;
        margin: auto;
        padding: 50px 0;
        text-align: center;

        h1 {
            font-size: 40px;
            margin-bottom: 30px;
        }

        input {
            width: 70%;
            padding: 20px;
        }

        button {
            background-color: #000;
            color: #fff;
            padding: 20px 100px;
            margin-left: 20px;
        }
    }
}

</style>
