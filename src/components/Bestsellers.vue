<template>
    <div class="container">
        <div class="flex-container">
            <div>
                <div class="green-title">All-time best sellers</div>
                <h3>Items everyone loves</h3>
            </div>
            <div>
                <a href="#" class="btn">View all product</a>
            </div>
        </div>

        <div class="flex-container">
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-21-600x600.jpg" alt="">
                    <div class="overlay-product">
                        <div class="content-product">
                            <div class="icon-container">
                                <font-awesome-icon icon="check-square" class="icon"/>
                            </div>
                            <div class="bold">view cart</div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Transport cage</div>
                <div class="product-price">$25.00</div>
            </div>
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-20-600x600.jpg" alt="">
                    <div class="overlay-product">
                        <div class="content-product">
                            <div class="icon-container">
                                <font-awesome-icon icon="check-square" class="icon"/>
                            </div>
                            <div class="bold">view cart</div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Dog leash</div>
                <div class="product-price">$25.00</div>
            </div>
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-11-600x600.jpg" alt="">
                    <div class="overlay-product">
                        <div class="content-product">
                            <div class="icon-container">
                                <font-awesome-icon icon="check-square" class="icon"/>
                            </div>
                            <div class="bold">view cart</div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Animal transport cage</div>
                <div class="product-price"><span class="deleted">$35.00</span>$25.00</div>
            </div>
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-16-600x600.jpg" alt="">
                    <div class="overlay-product">
                        <div class="content-product">
                            <div class="icon-container">
                                <font-awesome-icon icon="check-square" class="icon"/>
                            </div>
                            <div class="bold">view cart</div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Colorful cat leash</div>
                <div class="product-price">$25.00</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Bestsellers',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

.flex-container {
    justify-content: space-between;
    align-items: center;
    margin-bottom: 100px;

    h3 {
        margin: 30px 0 0 0;
    }

    .flex-item {
        width: 23%;
        text-align: center;
    }
}
</style>