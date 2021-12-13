<template>
<!-- N.B. Creare gli elementi per ogni sezione -->
    <div>
        <!-- jumbotron -->
        <Jumbotron/>

        <!-- primo blocco main -->
        <section>
            <!-- titolo -->
            <!-- immagini -->
                <!-- img/title/date/comments/description -->
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
        <!-- break-line blog-->
        <section>
            <!-- title -->
            <div>
                <!-- blog section x8 -->
            </div>
        </section>
        <!-- break-line forum -->
        <section>
            <!-- title -->
            <!-- text -->
            <!-- button -->
        </section>
        <!-- NEWSLETTER -->
        <section>
            <!-- title -->
            <!-- text area -->
            <!-- button -->
        </section>
    </div>
</template>

<script>
import Jumbotron from '@/components/Jumbotron.vue'

export default {
name: 'Main',
components: {
    Jumbotron
}
}

</script>

<style scoped lang="scss">

</style>