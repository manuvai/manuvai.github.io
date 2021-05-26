<template>
  <div id="app">
    <NavBar/>
    <Introduction/>
    <About/>
    <Works/>
    <Contact/>
  </div>
</template>

<script>
import Vue from 'vue';
import NavBar from './components/NavBar'
import Contact from './components/Contact'
import Introduction from './components/Introduction'
import About from './components/About'
import Works from './components/Works'
import VueRellax from 'vue-rellax'

Vue.use(VueRellax)
export default {
  created () {
  },
  name: 'app',
  components: {
    NavBar,
    Contact,
    Introduction,
    About,
    Works,
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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
