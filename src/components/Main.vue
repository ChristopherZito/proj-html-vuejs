<template>
<!-- N.B. Creare gli elementi per ogni sezione -->
    <div>
        <!-- jumbotron -->
        <Jumbotron/>
        <!-- main part -->
        <News/>
        <!-- break-line blog-->
        <Blog/>
        <!-- break-line forum -->
        <Forum/>
        <!-- NEWSLETTER -->
        <NewsLetter/>
    </div>
</template>

<script>
import Jumbotron from '@/components/Jumbotron.vue'
import News from '@/components/News.vue'
import Blog from '@/components/Blog.vue'
import Forum from '@/components/Forum.vue'
import NewsLetter from '@/components/NewsLetter.vue'

export default {
name: 'Main',
components: {
    Jumbotron,
    News,
    Blog,
    Forum,
    NewsLetter,
}
}

</script>

<style scoped lang="scss">

</style>