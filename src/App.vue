<template>
  <div id="app">
    <Header
      :navList="headerNavList"
    />
    <Jumbo/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbo from './components/Jumbo.vue'

export default {
  name: 'App',
  components: {
    Header,
    Jumbo
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
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  width: 75%;
  margin: 0 auto;
}

.btn {
  display: inline-block;
  padding: 15px 25px;
  border-radius: 30px;
  background-color: $btn-green;
  color: white;
  text-decoration: none;
}

.bold {
  font-weight: bold;
}
</style>
