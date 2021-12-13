<template>
    <main>
        <BrowseByCategory/>
        <NewArrivals/>
    </main>
</template>

<script>
import BrowseByCategory from '@/components/BrowseByCategory.vue'
import NewArrivals from '@/components/NewArrivals.vue'

export default {
    name: 'Main',
    components: {
        BrowseByCategory,
        NewArrivals
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";


</style>