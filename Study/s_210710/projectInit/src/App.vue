<template>


<div id="app">

  <div class="wrap">

     <header-component></header-component>
     <main-component></main-component>
     <footer-component></footer-component>

     <!--<headerComponent>와 같은 카멜기법으로 작성도 가능 /cli 한정-->

  </div>

</div>



</template>

<script>

// 컴포넌트 등록 

import headercomponent from './components/headerComponent.vue'
import maincomponent from './components/mainComponent.vue'
import footercomponent from './components/footerComponent.vue'

export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },components:{
    //가상 컴포넌트 등록 (템플릿에 외부파일 가져온 것 등록)
    'header-component' : headercomponent,
    'main-component' : maincomponent,
    'footer-component' : footercomponent

  }
}
</script>

<style>

*{margin: 0; padding: 0;vertical-align: middle; border:0;}
html,body{width:100%; height: 100%;}
body{font:normal 16px/1 'arial','고딕';color: #444; background: #fff;}
a{color:#444; text-decoration: none;}
li,ul{list-style: none;}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  _margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
