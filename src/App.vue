<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <functional-component 
     :brands ="['Tesla', 'Bentley', 'Ferrari', 'Ford']">
    </functional-component>
  </div>
</template>

<script>
import FunctionalComponent from './components/FunctionalComponent.vue'

export default {
  name: 'App',
  components: {
    FunctionalComponent
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
