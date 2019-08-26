<template>
  <div id="app">
    <TextWindow></TextWindow>
    <StatusBar></StatusBar>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
//import TerminalWindow from './components/TerminalWindow.vue'
import StatusBar from './components/StatusBar.vue'
import TextWindow from './components/TextWindow.vue'

export default {
  name: 'app',
  components: {
      StatusBar,
      TextWindow
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



