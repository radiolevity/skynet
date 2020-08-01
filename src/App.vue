<template>
  <div id="app">
    <Navbar />
  </div>
</template>

<script lang="ts">
  import { Component, Vue } from "vue-property-decorator";
  import HelloWorld from "./components/HelloWorld.vue";
  import Navbar from "./components/Navbar.vue";

  @Component({
    components: {
      Navbar,
      HelloWorld
    }
  })
  export default class App extends Vue {}
</script>

<style lang="scss">
  @import "scss/_variables.scss";
  // Import Bulma and Buefy styles
  @import "~bulma";
  @import "~buefy/src/scss/buefy";

  #app {
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
</style>
