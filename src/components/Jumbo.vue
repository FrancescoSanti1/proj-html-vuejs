<template>
    <section id="jumbo">
        <div id="jumbo-top">
            <div class="container flex-container">
                <div>
                    <font-awesome-icon icon="map" class="icon"/>
                    <span class="text"><span class="bold">International</span> Shipping Services</span>
                </div>
                <div>
                    <font-awesome-icon icon="clock" class="icon"/>
                    <span class="text">See out <span class="bold">store hours</span> and services</span>
                </div>
                <div>
                    <font-awesome-icon icon="check" class="icon"/>
                    <span class="text">We price match to give you the <span class="bold">best deals</span></span>
                </div>
            </div>
        </div>
        <div id="jumbo-main">
            <div class="overlay">
                <div class="container">
                    <div class="content">
                        <div class="uppercase-title">find the best animal supplies</div>
                        <h1>We know animals are a part of your family, let us help take care of them.</h1>
                        <a href="#" class="btn white">Learn more about us</a>
                    </div>
                </div>
            </div>
        </div>
        <div id="jumbo-bottom">
            <div class="container flex-container">
                <img src="../assets/img/food-transparent-5-400x223.png" alt="">
                <div>GET $25 OFF your first purchase of our homemade pet food!</div>
                <a href="#">Visit the shop</a>
            </div>
        </div>
        <div class="jumbo-btns">
            <div class="jumbo-btn">
                <font-awesome-icon icon="folder-open" class="icon"/>
                <div>Demos</div>
            </div>
            <div class="jumbo-btn">
                <div class="sale bold"><sup>$</sup>39</div>
                <div>On Sale</div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Jumbo',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

section {
    color: white;
    position: relative;
}

#jumbo-top {
    background: $dark-green;
    background-image: url('../assets/img/bg-transparent-3.png');
    height: 60px;

    .container.flex-container {
        height: 100%;
        justify-content: space-around;
        align-items: center;

        .icon {
            margin: 0 10px;
        }

        .text {
            color: #dcd5d0;

            .bold {
                color: white;
            }
        }
    }
}

#jumbo-main {
    background-image: url("../assets/img/banner-5-2x-scaled.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;

    .content {
        padding: 200px 0;
        width: 50%;
    }
}

#jumbo-bottom {
    background: $dark-green;
    background-image: url('../assets/img/bg-transparent-3.png');
    height: 150px;

    .container.flex-container {
        height: 100%;
        justify-content: center;
        align-items: center;

        img {
            height: 120px;
            align-self: flex-end;
        }

        div {
            margin: 0 20px;
        }

        a {
            color: #dcd5d0;
        }
    }
}

.jumbo-btns {
    position: absolute;
    top: 10px;
    right: 10px;

    .jumbo-btn {
        width: 70px;
        height: 70px;
        border-radius: 10px;
        margin-bottom: 10px;
        padding: 5px;
        background-color: $light-grey;
        text-align: center;
        color: $dark-grey;
        cursor: pointer;

        .icon {
            font-size: 2rem;
        }

        .sale {
            color: yellowgreen;
            font-size: 2.5rem;
        }
    }
}
</style>