<template>
  <div>
    <h2>Bài 1</h2>
    <img :src="image" alt="">
  </div>
</template>

<script setup>
let image='https://i.pinimg.com/564x/4a/4c/0e/4a4c0ef22c89c4a504fb0ee8d420b996.jpg'
</script>

<style scoped>
img{
    width: 200px;
    height: 200px;
}
</style>