<template>
    <section class="container">
        <h3>Get the best tips &amp; tricks</h3>
        <div class="green-title">Recent articles</div>
        <div class="flex-container">
            <div class="flex-item">
                <div class="img-container">
                    <img src="../assets/img/blog-1-600x600.jpg" alt="">
                    <div class="overlay">
                        <div class="content">
                            <div class="overlay-title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                            <div>Tips &amp; tricks</div>
                        </div>
                    </div>
                </div>
                <div class="title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                <div class="date">April 21st, 2020</div>
            </div>
            <div class="flex-item">
                <div class="img-container">
                    <img src="../assets/img/blog-2-600x600.jpg" alt="">
                    <div class="overlay">
                        <div class="content">
                            <div class="overlay-title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                            <div>Tips &amp; tricks</div>
                        </div>
                    </div>
                </div>
                <div class="title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                <div class="date">April 21st, 2020</div>
            </div>
            <div class="flex-item">
                <div class="img-container">
                    <img src="../assets/img/blog-3-600x600.jpg" alt="">
                    <div class="overlay">
                        <div class="content">
                            <div class="overlay-title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                            <div>Tips &amp; tricks</div>
                        </div>
                    </div>
                </div>
                <div class="title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                <div class="date">April 21st, 2020</div>
            </div>
            <div class="flex-item">
                <div class="img-container">
                    <img src="../assets/img/blog-4-600x600.jpg" alt="">
                    <div class="overlay">
                        <div class="content">
                            <div class="overlay-title">How to &lsquo;loose leash walk&rsquo; tour dog</div>
                            <div>Tips &amp; tricks</div>
                        </div>
                    </div>
                </div>
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

    .flex-container {
        justify-content: space-between;
        margin: 40px 0;
    
        .flex-item {
            width: 23%;
            text-align: left;

            .img-container {
                position: relative;

                .overlay {
                    position: absolute;
                    top: 0;
                    right: 0;
                    bottom: 0;
                    left: 0;
                    justify-content: center;
                    align-items: center;
                    background-color: rgba($color: #c27548, $alpha: 0.4);
                    display: none;

                    .content {
                        text-align: center;
                        color: white;
                        width: 70%;

                        .overlay-title {
                            font-size: 1.3rem;
                            margin-bottom: 10px;
                        }
                    }
                }

                img {
                    width: 100%;
                    display: block;
                }

                &:hover {

                    .overlay {
                    display: flex;
                    }
                }
            }

            &:hover {
                cursor: pointer;
            }

            .title, .date {
                padding: 0 30px;
            }

            .title {
                line-height: 2rem;
                margin-top: 20px;
            }

            .date {
                font-size: 0.8rem;
                color: $dark-grey;
            }
        }
    }
}
</style>