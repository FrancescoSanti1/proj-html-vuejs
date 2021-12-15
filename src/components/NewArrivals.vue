<template>
    <section>
        <div class="container">
            <div class="overlay">
                <div class="content">
                    <div class="uppercase-title">find the best animal supplies</div>
                    <h2>New arrivals weekly</h2>
                    <a href="#" class="btn white">Learn more about us</a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'NewArrivals',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

.container {
    background-image: url("../assets/img/banner-3-2x-scaled.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    margin: 100px auto;

    .content {
        padding: 150px 0;
        text-align: center;
        color: white;
    }
}
</style>