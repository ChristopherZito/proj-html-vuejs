<template>
<!-- N.B. Creare gli elementi per ogni sezione -->
    <div>
        <!-- jumbotron -->
        <Jumbotron/>
        <!-- main part -->
        <News/>
        <!-- break-line blog-->
        <Forum/>
        <!-- break-line forum -->
        <Community/>
        <!-- NEWSLETTER -->
        <NewsLetter/>
    </div>
</template>

<script>
import Jumbotron from '@/components/Jumbotron.vue'
import News from '@/components/News.vue'
import Forum from '@/components/Forum.vue'
import Community from '@/components/Community.vue'
import NewsLetter from '@/components/NewsLetter.vue'

export default {
name: 'Main',
components: {
    Jumbotron,
    News,
    Forum,
    Community,
    NewsLetter,
}
}

</script>

<style scoped lang="scss">

</style>