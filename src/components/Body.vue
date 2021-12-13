<template>
    <section>
        <header>
            <Header/>
        </header>
        <main>
            <Main/>
        </main>
        <footer>
            <Footer/>
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
    }
}
</script>

<style scoped lang="scss">

</style>