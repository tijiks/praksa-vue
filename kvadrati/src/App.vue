<template>
  <Square />
  <Square />
  <Square />
</template>

<script>

import Square from './components/Square.vue'

export default {
  name: 'App',
  components: {Square}
  
}
</script>

<style>
body{
  background: yellow;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
