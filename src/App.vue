<template>

<navbar-vue></navbar-vue>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="WENA Cabrosss"/>
<footer-vue></footer-vue>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import navbarVue from './components/navbar.vue'
import footerVue from './components/footer.vue';
import 'bootstrap'; 
import 'bootstrap/dist/css/bootstrap.min.css'

export default {
  name: 'App',
  components: {
    HelloWorld,
    navbarVue,
    footerVue
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
}
</style>
