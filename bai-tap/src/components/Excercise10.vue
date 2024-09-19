<template>
  <div>
    <h2>Bài 10</h2>
    <input @keyup.enter="handleChange" type="text" v-model="textInput">
  </div>
</template>

<script setup>
  import { ref } from 'vue';
   const textInput=ref('');
   const handleChange=(e)=>{
       if(e.shiftKey){
        alert(textInput.value);
        textInput.value='';
       }else{
        alert('Bạn cần nhấn shift và enter')
       }
   }
</script>

<style>

</style>