<template>
    <section>
        <div class="background">
            <h3>Testimonials</h3>
            <div class="testimonials container flex-container">
                <div class="flex-item">
                    <div class="img-container">
                        <img src="../assets/img/avatar-3-200x200.jpg" alt="">
                    </div>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusantium ea facilis voluptates officia et reiciendis.</p>
                    <div class="author">Lisa Smith, ThemeFusion</div>
                </div>
                <div class="flex-item">
                    <div class="img-container">
                        <img src="../assets/img/avatar-1-200x200.jpg" alt="">
                    </div>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusantium ea facilis voluptates officia et reiciendis.</p>
                    <div class="author">Lisa Smith, ThemeFusion</div>
                </div>
                <div class="flex-item">
                    <div class="img-container">
                        <img src="../assets/img/avatar-4-200x200.jpg" alt="">
                    </div>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusantium ea facilis voluptates officia et reiciendis.</p>
                    <div class="author">Lisa Smith, ThemeFusion</div>
                </div>
            </div>
        </div>
        <div class="newsletter container">
            <div class="content">
                <h3>Join our newsletter</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Minima omnis sequi quae sapiente assumenda architecto temporibus earum, nesciunt magni asperiores cupiditate ducimus.</p>
                <input type="text" placeholder="Insert your e-mail...">
                <span class="btn">Subscribe</span>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'TestimonialsAndNewsletter',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";
.background {
    text-align: center;
    background-color: $dark-green;
    color: white;
    padding: 100px 0 200px;

    h3 {
        margin: 0 0 50px;
    }

    .testimonials.flex-container {
        justify-content: space-around;

        .flex-item {
            width: 30%;

            .img-container {
                width: 150px;
                height: 150px;
                margin: 0 auto 20px;
                border-radius: 50%;
                overflow: hidden;

                img {
                    width: 100%;
                }
            }

            p {
                line-height: 2rem;
            }

            .author {
                color: $dark-grey;
                margin-top: 30px;
            }
        }    
    }
}

.newsletter.container {
    background-image: url("../assets/img/banner-7-2x-scaled.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    margin-top: -50px;

    .content {
        padding: 100px 0 100px 100px;
        width: 50%;

        h3 {
            margin-top: 0;
        }

        p {
            line-height: 2rem;
            color: $dark-grey;
            margin-bottom: 30px;
        }

        input {
            padding: 15px 25px;
            background-color: $light-grey;
            border-radius: 30px;
            border: none;
            margin-right: 20px;
        }
    }
}
</style>