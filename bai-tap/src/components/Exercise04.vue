<template>
    <div>
        <h2>Bài 4</h2>
  <div :class="{active:isActive}" :style="{backgroundColor: bg}">
     Block
  </div>
  <button v-on:click="handleClick">Change</button>
   </div>
</template>

<script setup>
import {ref} from 'vue'
let bg=ref('green');
let isActive=ref(false);
const handleClick=()=>{
    isActive.value=!isActive.value;
    bg.value=bg.value=='red'?'green':'red';
}
</script>

<style>
.active{
    color:white;
}
</style>