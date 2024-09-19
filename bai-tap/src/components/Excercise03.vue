<template>
  <div>
    <h2>Bài 3</h2>
    <input :disabled="isDisabled" type="text">
    <button v-on:click="handleClick">Change</button>
  </div>
</template>

<script setup>
import {ref} from 'vue'
let isDisabled =ref(false);
const handleClick=()=>{
    isDisabled.value=!isDisabled.value;
}
</script>

<style scoped>

</style>