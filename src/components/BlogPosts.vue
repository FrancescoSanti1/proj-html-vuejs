<template>
    <section class="container">
        <h3>Get the best tips &amp; tricks</h3>
        <div class="subtitle">Recent articles</div>
        <div class="flex-container">
            <div class="flex-item">
                <img src="../assets/img/blog-1-600x600.jpg" alt="">
                <div class="title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                <div class="date">April 21st, 2020</div>
            </div>
            <div class="flex-item">
                <img src="../assets/img/blog-2-600x600.jpg" alt="">
                <div class="title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                <div class="date">April 21st, 2020</div>
            </div>
            <div class="flex-item">
                <img src="../assets/img/blog-3-600x600.jpg" alt="">
                <div class="title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                <div class="date">April 21st, 2020</div>
            </div>
            <div class="flex-item">
                <img src="../assets/img/blog-4-600x600.jpg" alt="">
                <div class="title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                <div class="date">April 21st, 2020</div>
            </div>
        </div>
        <a href="#" class="btn">Read all articles</a>
    </section>
</template>

<script>
export default {
    name: 'BlogPosts',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

.container {
    text-align: center;

    h3 {
        margin-bottom: 20px;
    }

    .subtitle {
        color: $btn-green;
    }

    .flex-container {
        justify-content: space-between;
        margin: 40px 0;
    
        .flex-item {
            width: 23%;
            text-align: left;

            img {
                width: 100%;
            }

            .title, .date {
                padding: 0 30px;
            }

            .title {
                line-height: 2rem;
            }

            .date {
                font-size: 0.8rem;
                color: $dark-grey;
            }
        }
    }
}
</style>