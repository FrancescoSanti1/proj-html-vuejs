<template>
    <div class="container">
        <h3>Browse by category</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem quas eum error aut nihil qui sed in repellat minus dicta eius accusamus deserunt perspiciatis ex facilis amet, dolor placeat earum?</p>
        <div class="flex-container">
            <div class="flex-item">
                <img src="../assets/img/product-9-500x500.jpg" alt="">
                <div class="product-name">Bed (1)</div>
            </div>
            <div class="flex-item">
                <img src="../assets/img/product-3-500x500.jpg" alt="">
                <div class="product-name">Food (6)</div>
            </div>
            <div class="flex-item">
                <img src="../assets/img/product-2-500x500.jpg" alt="">
                <div class="product-name">Toys (6)</div>
            </div>
            <div class="flex-item">
                <img src="../assets/img/product-4-500x500.jpg" alt="">
                <div class="product-name">Transport (6)</div>
            </div>
        </div>

        <div class="flex-container">
            <div class="flex-item green">
                <h3>Kibble</h3>
                <p class="green-title">Dry dog food</p>
                <img src="../assets/img/food-transparent-18.png" alt="">
                <a href="#" class="btn">Shop dry food</a>
            </div>
            <div class="flex-item green">
                <h3>Moist</h3>
                <p class="green-title">Canned dog food</p>
                <img src="../assets/img/food-transparent-17.png" alt="">
                <a href="#" class="btn">Shop moist food</a>
            </div>
            <div class="flex-item green">
                <h3>Frozen</h3>
                <p class="green-title">Freeze-Dried dog food</p>
                <img src="../assets/img/food-transparent-16.png" alt="">
                <a href="#" class="btn">Shop frozen food</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'BrowseByCategory',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

.container {
    text-align: center;

    p {
        width: 50%;
        margin: 0 auto 50px;
        line-height: 30px;
    }

    .flex-container {
        justify-content: space-between;

        .flex-item {
            width: 24%;

            img {
                width: 100%;
            }

            .product-name {
                margin-top: 20px;
            }
        }

        .flex-item.green {
            width: 32%;
            background-color: $dark-green;
            margin-top: 50px;
            padding: 40px 0;

            &:hover {
                transform: scale(1.05);
                box-shadow: 0 0 20px rgba(0, 0, 0, 0.6);
                cursor: pointer;
            }

            h3 {
                margin: 0 0 20px;
                color: white;
            }

            p {
                color: $btn-green;
            }

            img {
                display: block;
                width: 60%;
                margin: 0 auto;
            }

            .btn:hover {
                background-color: $btn-green;
                color: white;
            }
        }
    }
}
</style>