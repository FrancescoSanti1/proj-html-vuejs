<template>
    <header>
        <div id="header-top">
            <div class="container flex-container">
                <div id="logo">
                    <img src="../assets/img/dark-pet-logo.png" alt="logo">
                </div>
                <div id="search-bar">
                    <font-awesome-icon icon="search" class="icon"/>
                    <input type="text" placeholder="Search...">
                </div>
                <div><span class="bold">Questions?</span> Call us: 1.800.123.4567</div>
                <div class="icons">
                    <font-awesome-icon icon="shopping-bag" class="icon"/>
                    <font-awesome-icon icon="user" class="icon"/>
                </div>
            </div>
        </div>
        <nav>
            <ul>
                <li v-for="item, i in navList" :key="item.linkName" :class="i === selectedMenuItem ? 'active' : ''">
                    <a :href="item.linkPath" 
                    class="bold" 
                    @click="changeSelectedMenuItem(i)"
                    >{{item.linkName}}</a>
                    <span v-if="item.subMenu.length !== 0">
                        <font-awesome-icon icon="chevron-down" class="icon"/>
                    </span>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Header',
    props: {
        navList: Array
    },
    data() {
        return {
            selectedMenuItem: 0
        }
    },
    methods: {
        changeSelectedMenuItem(index) {
            this.selectedMenuItem = index;
            this.$emit('changeSelectedMenuItem', this.selectedMenuItem);
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/_variables.scss";

header {

    #header-top {
        border-bottom: 1px solid #dcd5d0;

        .container.flex-container {
            height: 80px;
            justify-content: space-between;
            align-items: center;

            #logo {
                img {
                    height: 40px;
                }
            }

            #search-bar {
                background-color: $light-grey;
                padding: 10px 20px;
                border-radius: 20px;

                input {
                    background-color: $light-grey;
                    border: none;
                    width: 300px;
                }
            }

            .icon {
                margin-right: 10px;
            }

            .icons .icon {
                font-size: 1.5rem;
                margin: 0 10px;

                &:hover {
                    transform: scale(1.2);
                    cursor: pointer;
                }
            }
        }
    }

    nav {
        height: 60px;

        ul {
            height: 100%;
            margin: 0 auto;
            display: flex;
            justify-content: center;
            align-items: center;

            li {
                margin: 0 10px;
                color: $dark-grey;

                a {
                    color: $dark-grey;
                    padding: 10px;
                }

                &.active {
                    color: black;

                    a {
                        color: black;
                    }
                }
            }
        }
    }
}

</style>
