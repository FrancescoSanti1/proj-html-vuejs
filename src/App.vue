<template>
  <div id="app">
    <Header
      :navList="headerNavList"
    />
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
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

.bold {
  font-weight: bold;
}
</style>
