<template>
    <div class="square-styl">
       <p>{{text}}</p> 
    </div>
</template>
<script>
    export default{
        name: 'Square',
        props:['text']
    }
</script>
<style>
    .square-styl{
        background: blue;
        width:300px;
        height:300px;          
    }
    p{ margin-top:50%;
        color:white;}
</style>