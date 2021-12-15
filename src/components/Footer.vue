<template>
    <footer>
        <div id="footer-main">
            <div class="container">
                <div class="flex-container">
                    <div class="flex-item">
                        <img src="../assets/img/mobile-light-pet-logo-2x.png" alt="logo">
                        <p>1234 Avada Avenue Avadaville<br>info&commat;company.com<br>Call us: 0123 345 6789</p>
                    </div>
                    <div class="flex-item">
                        <h5>Shop by brand</h5>
                        <ul>
                            <li v-for="item in brandsList" :key="item.linkName">
                                <a :href="item.linkPath">{{item.linkName}}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="flex-item">
                        <h5>Useful links</h5>
                        <ul>
                            <li v-for="item in usefulLinksList" :key="item.linkName">
                                <a :href="item.linkPath">{{item.linkName}}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="flex-item subscribe">
                        <h5>Subscribe to our newsletter</h5>
                        <input type="text" placeholder="insert your e-mail...">
                        <div class="btn">Subscribe</div>
                    </div>
                </div>

                <nav>
                    <ul>
                        <li v-for="item, i in navList" :key="item.linkName">
                            <a :href="item.linkPath" :class="i === selectedMenuItem ? 'active' : ''">{{item.linkName}}</a>
                        </li>
                    </ul>
                </nav>
                <div class="icons">
                    <font-awesome-icon :icon="['fab', 'facebook-f']" class="icon"/>
                    <font-awesome-icon :icon="['fab', 'twitter']" class="icon"/>
                    <font-awesome-icon :icon="['fab', 'instagram']" class="icon"/>
                    <font-awesome-icon :icon="['fab', 'youtube']" class="icon"/>
                </div>
            </div>
        </div>
        <div id="footer-bottom">
            <p>&copy; Copyright 2021 - Avada Theme by ThemeFusion | All Rights Reserved</p>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    props: {
        brandsList: Array,
        usefulLinksList: Array,
        navList: Array,
        selectedMenuItem: Number
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

#footer-main {
    background-color: $dark-green;
    padding: 100px 0;

    .flex-container {
        color: white;
        padding-bottom: 30px;
        border-bottom: $dark-grey 1px solid;

        .flex-item {
            width: 25%;

            img {
                width: 70%;
            }
            
            p {
                line-height: 2rem;
                margin-top: 30px;
            }

            h5 {
                margin-bottom: 40px;
            }

            ul {

                li {
                    margin: 20px 0;

                    a {
                        color: white;

                        &:hover {
                            text-decoration: underline;
                        }
                    }
                }
            }

            &.subscribe {
                background: #264229;
                background-image: url('../assets/img/bg-transparent-3.png');
                padding: 30px;

                input {
                    width: 100%;
                    padding: 15px 25px;
                    margin-bottom: 30px;
                    background-color: $light-grey;
                    border-radius: 30px;
                    border: none;
                }

                .btn {
                    display: block;
                    text-align: center;
                }
            }
        }
    }

    nav {
        text-align: center;

        ul {

            li {
                display: inline-block;
                margin: 50px 10px;

                a {
                    color: $dark-grey;

                    &.active {
                        color: white;
                    }

                    &:hover {
                        text-decoration: underline;
                        color: white;
                    }
                }
            }
        }
    }

    .icons {
        text-align: center;

        .icon {
            color: white;
            margin: 0 10px;
            font-size: 1.2rem;

            &:hover {
                cursor: pointer;
                transform: scale(1.3);
            }
        }
    }
}

#footer-bottom {
    background-color: black;
    padding: 30px 0;
    
    p {
        text-align: center;
        color: white;
        font-size: 0.9rem;
    }
}
</style>