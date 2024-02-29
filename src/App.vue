<template>
  <div id="app">
    <ButtonFirst>Click me</ButtonFirst>
  </div>
</template>

<script>

import ButtonFirst from './components/ButtonFirst.vue';

export default {
  name: 'App',
  components: {
    ButtonFirst
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
