<template>
    <section class="jumbo">
        <div id="jumbo-top">
            <div class="container">
                <div>
                    <font-awesome-icon icon="map" class="icon"/>
                    <span class="bold">International</span> Shipping Services</div>
                <div>
                    <font-awesome-icon icon="clock" class="icon"/>
                    See out <span class="bold">store hours</span> and services</div>
                <div>
                    <font-awesome-icon icon="check" class="icon"/>
                    We price match to give you the <span class="bold">best deals</span></div>
            </div>
        </div>
        <div id="jumbo-main">
            <div class="overlay">
                <div class="container">
                    <div class="content">
                        <div>find the best animal supplies</div>
                        <h1>We know animals are a part of your family, let us help take care of them.</h1>
                        <a href="#" class="btn white">Learn more about us</a>
                    </div>
                </div>
            </div>
        </div>
        <div id="jumbo-bottom">
            <div class="container">
                <img src="../assets/img/food-transparent-5-400x223.png" alt="">
                <div>GET $25 OFF your first purchase of our homemade pet food!</div>
                <a href="#">Visit the shop</a>
            </div>
        </div>
        <div class="jumbo-btns">
            <div class="jumbo-btn">Demos</div>
            <div class="jumbo-btn">On sale</div>
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
    background-color: $dark-green;
    height: 60px;

    .container {
        height: 100%;
        display: flex;
        justify-content: space-around;
        align-items: center;

        .icon {
            margin: 0 10px;
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

        div {
            text-transform: uppercase;
        }
    }
}

#jumbo-bottom {
    background-color: $dark-green;
    height: 150px;

    .container {
        height: 100%;
        display: flex;
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
    }
}
</style>