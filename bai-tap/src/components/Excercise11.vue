<template>
  <div>
     <h2>Bài 11</h2>
     <div class="box" :style="{backgroundColor:color}"></div>
     <button @click="handleChange">Change</button>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const color=ref('red');
const handleChange=()=>{
    color.value=color.value==='red'?'blue':'red';
}
</script>

<style scoped>
.box{
    width: 100px;
    height: 100px;
    transition: background-color 0.5s ease;
}
</style>