<template>
  <div id="app">
      
      <header-component></header-component>
      <input-component></input-component>
      <list-component></list-component>
      <footer-component></footer-component>

  </div>
</template>

<script>
import HeaderComponent from './components/headerComponent.vue'
import InputComponent from './components/inputComponent.vue'
import ListComponent from './components/ListComponent.vue'
import FooterComponent from './components/footerComponent.vue'

export default {
  name: 'App',
  components: {
    'header-component' : HeaderComponent,
    'input-component' : InputComponent,
   'list-component' : ListComponent,
   'footer-component' : FooterComponent
  }
}
</script>

<style>

</style>
