<template>
    <div>
    <h2>Bài 6</h2>
     <button @click="handleClick('Rikkei Academy')">Get Param</button>
    </div>
</template>

<script setup>
    const handleClick=(str)=>{
       console.log(str);      
    }
</script>

<style>

</style>