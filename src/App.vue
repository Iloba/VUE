<template>
<loop/>
<kaye/>
<jude msg="Ebeke Component" />
<Home />
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your  Vue.js + Laravel App"/>
  
  
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Home from './components/Home.vue'
import Jude from './components/Jude.vue'
import Kaye from './components/Kaye.vue'
import Loop from './components/Loop.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Home,
    Jude,
    Kaye,
    Loop
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
