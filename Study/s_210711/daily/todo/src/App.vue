<template>
  <div id="app">
      <header-component></header-component>
      <main-component></main-component>
      <footer-component></footer-component>

  </div>
</template>

<script>

import FooterComponent from './components/footerComponent.vue'
import HeaderComponent from './components/headerComponent.vue'
import MainComponent from './components/mainComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent 
  }
}
</script>

<style>

*{padding: 0; margin: 0;}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}


</style>
