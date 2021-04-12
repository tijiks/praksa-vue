<template>
<div id="horizontal">
  
    <Square @click="ispis='1'"></Square>
    <Square  :text="ispis" @click="ispis='2'"><p>{{ispis}}</p></Square>
    <Square @click="ispis='3'"></Square>
 
</div>
</template>

<script>

import Square from './components/Square.vue'

export default {
  name: 'App',
  components: {Square},
  data(){
    return{
      ispis:""
     
    }

  },
  
 

  
}
</script>

<style>
body{
  background: yellow;
}
#horizontal{
  display:flex;
  justify-content: space-around;
  margin-top:10%;
  margin-bottom:10%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
 
 
 
  
}
</style>
