<template>
    <section>
        <div class="view-all flex-container">
            <div class="flex-item popular">
                <div class="overlay">
                    <div class="content">
                        <div class="subtitle bold">find the best animal supplies</div>
                        <h3>Popular accessories</h3>
                        <a href="#" class="btn white">View all toys accessories</a>
                    </div>
                </div>
            </div>
            <div class="flex-item new">
                <div class="overlay">
                    <div class="content">
                        <div class="subtitle bold">find the best food</div>
                        <h3>New food arrival</h3>
                        <a href="#" class="btn white">View all food products</a>
                    </div>
                </div>
            </div>
        </div>
        <div class="icons-background">
            <div class="container flex-container">
                <div class="flex item">
                    <font-awesome-icon icon="truck" class="icons"/>
                    <div class="text">Free worldwide deliveries</div>
                </div>
                <div class="flex item">
                    <font-awesome-icon icon="map" class="icons"/>
                    <div class="text">Free worldwide deliveries</div>
                </div>
                <div class="flex item">
                    <font-awesome-icon icon="dollar-sign" class="icons"/>
                    <div class="text">Free worldwide deliveries</div>
                </div>
                <div class="flex item">
                    <font-awesome-icon icon="credit-card" class="icons"/>
                    <div class="text">Free worldwide deliveries</div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'BannerViewallAndIcons',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

section {
    margin: 100px 0;
}

.view-all.flex-container {

    .flex-item {
        width: 50%;
        color: white;
        background-size: cover;
        background-repeat: no-repeat;

        &.popular {
            background-image: url("../assets/img/banner-8-2x.jpg");
        }

        &.new {
            background-image: url("../assets/img/banner-9-2x.jpg");
        }

        .content {
            padding: 150px 0;
            width: 40%;
            margin: 0 auto;
            text-align: center;

            .subtitle {
                text-transform: uppercase;
                font-size: 0.9rem;
            }

            h3 {
                margin: 30px 0 50px;
            }
        }
    }
}

.icons-background {
    background-color: $dark-green;
    padding: 100px 0;

    .flex-container {
        justify-content: space-around;
        text-align: center;

        .flex.item {
            width: 22%;

            .icons {
                font-size: 3rem;
                color: white;
            }

            .text {
                color: $dark-grey;
                margin-top: 10px;
            }
        }
    }
}
</style>