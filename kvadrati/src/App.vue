<template>
<div id="horizontal">
  
    <Square v-for="square in squares" :key="square.id" @squareClicked="squareClicked" 
    :id="square.id" 
    :text="square.text" 
    :color="square.color"
    ></Square>
 
</div>
</template>

<script>

import Square from './components/Square.vue'

export default {
  name: 'App',
  components: {Square},
  data(){
    return{
      squares:[
        {
          id: 1,
          text:'',
          color:'blue'

        },
        {
          id: 2,
          text:'',
          color:'blue'

        },
        {
          id: 3,
          text:'',
          color:'blue'

        },
      ]
      
    }
  },
  methods:{
        squareClicked: function(id){
        this.squares[1].text=id;
         this.squares.forEach(s => {
          if(s.id===id){
             s.color='red';
          }
          else{
            s.color='blue';
          }
         })
          
        }
      }
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
