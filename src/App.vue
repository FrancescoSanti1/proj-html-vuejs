<template>
  <div id="app">
    <Header
      :navList="headerNavList"
    />
    <Jumbo/>
    <Main/>
    <Footer/>
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
      headerNavList: [
        {linkName: "Home", linkPath: "#", subMenu: [{subLinkName: "Nome", subLinkPath: "#"}]},
        {linkName: "Shop", linkPath: "#", subMenu: [{subLinkName: "Nome", subLinkPath: "#"}]},
        {linkName: "About", linkPath: "#", subMenu: []},
        {linkName: "Blog", linkPath: "#", subMenu: []},
        {linkName: "Contact", linkPath: "#", subMenu: []},
        {linkName: "Shop by brand", linkPath: "#", subMenu: [{subLinkName: "Nome", subLinkPath: "#"}]}
      ]
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

.container {
    width: 75%;
    margin: 0 auto;
}
</style>
