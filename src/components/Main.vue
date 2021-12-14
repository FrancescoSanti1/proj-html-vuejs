<template>
    <main>
        <BrowseByCategory/>
        <NewArrivals/>
        <Bestsellers/>
        <TestimonialsAndNewsletter/>
        <BlogPosts/>
        <BannerViewallAndIcons/>
        <NewProducts/>
    </main>
</template>

<script>
import BrowseByCategory from '@/components/BrowseByCategory.vue'
import NewArrivals from '@/components/NewArrivals.vue'
import Bestsellers from '@/components/Bestsellers.vue'
import TestimonialsAndNewsletter from '@/components/TestimonialsAndNewsletter.vue'
import BlogPosts from '@/components/BlogPosts.vue'
import BannerViewallAndIcons from '@/components/BannerViewallAndIcons.vue'
import NewProducts from '@/components/NewProducts.vue'

export default {
    name: 'Main',
    components: {
        BrowseByCategory,
        NewArrivals,
        Bestsellers,
        TestimonialsAndNewsletter,
        BlogPosts,
        BannerViewallAndIcons,
        NewProducts
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";


</style>