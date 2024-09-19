<template>
    <div>
        <h2>Bài 9</h2>
        <button @click="handleClick">CLick {{ count }} lần</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';

   let count=ref(0);
   const handleClick=()=>{
     count.value++;
   }
</script>

<style>

</style>