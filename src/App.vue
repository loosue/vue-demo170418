<template>
  <div id="app">
    <hello></hello>
  </div>
</template>

<script>
import Hello from './components/Hello'

export default {
  name: 'app',
  components: {
    Hello
  }
}
</script>

<style>
html,body,header,footer,h1,h2,p,ul,li,div{padding: 0;margin: 0;}
h1, h2 {font-weight: normal;}
ul {list-style-type: none;}
li {display: inline-block;margin: 0 10px;}
a {text-decoration: none;color: #42b983;}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
