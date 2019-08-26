<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <TerminalWindow></TerminalWindow>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TerminalWindow from './components/TerminalWindow.vue'

export default {
  name: 'app',
  components: {
      TerminalWindow
  }
}
</script>

<style>
pre, html, body {
    margin: 0;
    padding: 0;
    height: 100%;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;
}
</style>



