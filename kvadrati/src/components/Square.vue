<template>
    <div class="square-styl" :style="`background-color: ${color}`" @click="onCLick">
       <p>{{text}}</p> 
    </div>
</template>
<script>
    export default{
        name: 'Square',
        props:["id","text","color"],
        methods:{
            onCLick: function(){
                this.$emit("squareClicked", this.id);
            }
        },


        }
        
</script>
<style>
    .square-styl{
        width:300px;
        height:300px;          
    }
    p{ margin-top:50%;
        color:white;}
</style>