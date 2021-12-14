<template>
    <section class="container">
        <h3>New products arrival</h3>
        <div class="green-title">Latest products</div>
        <div class="flex-container">
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-8-700x700.jpg" alt="">
                    <div class="overlay-product">
                        <div class="overlay-product">
                            <div class="content-product">
                                <div class="icon-container">
                                    <font-awesome-icon icon="check-square" class="icon"/>
                                </div>
                                <div class="bold">view cart</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Colored pet bed</div>
                <div class="product-price">$18.00 - $26.00</div>
            </div>
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-2-700x700.jpg" alt="">
                    <div class="overlay-product">
                        <div class="overlay-product">
                            <div class="content-product">
                                <div class="icon-container">
                                    <font-awesome-icon icon="check-square" class="icon"/>
                                </div>
                                <div class="bold">view cart</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Colorful ball set</div>
                <div class="product-price">$29.00</div>
            </div>
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-3-700x700.jpg" alt="">
                    <div class="overlay-product">
                        <div class="overlay-product">
                            <div class="content-product">
                                <div class="icon-container">
                                    <font-awesome-icon icon="check-square" class="icon"/>
                                </div>
                                <div class="bold">view cart</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Dog bone</div>
                <div class="product-price"><span class="deleted">$26.00</span>$18.00</div>
            </div>
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-4-700x700.jpg" alt="">
                    <div class="overlay-product">
                        <div class="overlay-product">
                            <div class="content-product">
                                <div class="icon-container">
                                    <font-awesome-icon icon="check-square" class="icon"/>
                                </div>
                                <div class="bold">view cart</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Animal transport bag</div>
                <div class="product-price">$29.00</div>
            </div>
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-5-700x700.jpg" alt="">
                    <div class="overlay-product">
                        <div class="overlay-product">
                            <div class="content-product">
                                <div class="icon-container">
                                    <font-awesome-icon icon="check-square" class="icon"/>
                                </div>
                                <div class="bold">view cart</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Animal transport cage</div>
                <div class="product-price">$35.00</div>
            </div>
            <div class="flex-item">
                <div class="img-product-container">
                    <img src="../assets/img/product-10-700x700.jpg" alt="">
                    <div class="overlay-product">
                        <div class="overlay-product">
                            <div class="content-product">
                                <div class="icon-container">
                                    <font-awesome-icon icon="check-square" class="icon"/>
                                </div>
                                <div class="bold">view cart</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="product-name">Closable cat litter</div>
                <div class="product-price">$16.00</div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'NewProducts',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

.container {
    text-align: center;

    .flex-container {
        justify-content: space-between;
        flex-wrap: wrap;
        margin-bottom: 100px;

        .flex-item {
            width: 32%;
            margin-top: 30px;
        }
    }
}
</style>