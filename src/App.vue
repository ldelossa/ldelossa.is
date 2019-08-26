<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <TerminalWindow></TerminalWindow> -->
    <TextArea class="text-area-left"></TextArea>
    <TextArea class="text-area-right"></TextArea>
    <StatusBar class="status-bar"></StatusBar>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TextArea from './components/TextArea.vue'
import StatusBar from './components/StatusBar.vue'

export default {
  name: 'app',
  components: {
      TextArea,
      StatusBar
  }
}
</script>

<style>
pre, html, body {
    margin: 0;
    padding: 0;
    height: 100%;
}
.text-area-left {
    //grid-area: text-area-left;
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 1;
    grid-row-end: 1;
}
.text-area-right {
    grid-area: text-area-right;
    grid-column-start: 2;
    grid-column-end: 3;
    grid-row-start: 1;
    grid-row-end: 1;
}
.status-bar {
    grid-area: status-bar;
    grid-column-start: 1;
    grid-column-end: 3;
    grid-row-start: 2;
    grid-row-end: 2;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;
  display: grid;
  grid-template-columns: 50% 50%;
  grid-template-rows: 97% 3%;
  grid-template-areas:
    "text-area-left text-area-right
     status-bar status-bar";
}
</style>



