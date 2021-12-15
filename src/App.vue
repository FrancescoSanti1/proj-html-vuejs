<template>
  <div id="app">
    <Header
      :navList="mainNavList"
      @changeSelectedMenuItem="changeSelectedMenuItem"
    />
    <Jumbo/>
    <Main/>
    <Footer
      :brandsList="brandsList"
      :usefulLinksList="usefulLinksList"
      :navList="mainNavList"
      :selectedMenuItem="selectedMenuItem"
    />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbo from './components/Jumbo.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Jumbo,
    Main,
    Footer
  },
  data() {
    return {
      mainNavList: [
        {linkName: "Home", linkPath: "#", subMenu: [{subLinkName: "Nome", subLinkPath: "#"}]},
        {linkName: "Shop", linkPath: "#", subMenu: [{subLinkName: "Nome", subLinkPath: "#"}]},
        {linkName: "About", linkPath: "#", subMenu: []},
        {linkName: "Blog", linkPath: "#", subMenu: []},
        {linkName: "Contact", linkPath: "#", subMenu: []},
        {linkName: "Shop by brand", linkPath: "#", subMenu: [{subLinkName: "Nome", subLinkPath: "#"}]}
      ],
      brandsList: [
        {linkName: "Bed", linkPath: "#"},{linkName: "Food", linkPath: "#"},{linkName: "Toys", linkPath: "#"},{linkName: "Transport", linkPath: "#"}
      ],
      usefulLinksList: [
        {linkName: "My account", linkPath: "#"},{linkName: "Orders", linkPath: "#"},{linkName: "Checkout", linkPath: "#"},{linkName: "Cart", linkPath: "#"}
      ],
      selectedMenuItem: 0
    }
  },
  methods: {
    changeSelectedMenuItem(item) {
      this.selectedMenuItem = item;
    }
  }
}
</script>

<style lang="scss">
@import "@/assets/styles/_variables.scss";

#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-size: 14px;
}
</style>
