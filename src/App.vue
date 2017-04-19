<template>
  <div id="app">
    <ul>
      <li><router-link to = '/foo'>Go to Foo</router-link></li>
      <li><router-link to = '/bar'>Go to Bar</router-link></li>
    </ul>
    <router-view></router-view>
  </div>
</template>

<script>
import Hello from './components/Hello'

const Foo = {template:'<div>this si Foo</div>'}
const Bar = {template:'<div>this si Bar</div>'}

const routes = [
  {path:'/foo',component: Foo},
  {path:'/bar',component: Bar}
]

const router = new VueRouter({
  routes: routes
});

const app = new Vue({
 router
}).$mount('#app')
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
