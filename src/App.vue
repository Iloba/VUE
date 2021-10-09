<template>
<Class/>
<loop :data="classes"/>
<button v-on:click="getData">Button</button>
<kaye lovemsg="I love you boo" lovesms="I love you bae"/>

<jude :msg="names" />
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
import Class from './components/Class.vue'

export default {
  name: 'App',
  data(){
    return{
      names: {
        first: 'emeka',
        second: 'Timothy',
        third: 'Iloba',
      },
      classes: 'SS3K',
    }
  },
  methods:{
   getData(){
        alert('getData');
    }
  },
  components: {
    HelloWorld,
    Home,
    Jude,
    Kaye,
    Loop,
    Class
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
