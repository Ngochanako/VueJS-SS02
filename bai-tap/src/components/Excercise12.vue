<template>
    <div>
        <h2>Bài 12</h2>
        <img :src="image" alt="">
        <button @click="handleClick">Random Image</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';
    const listImages=["https://i.pinimg.com/564x/bf/ba/4d/bfba4df228e5639b62dce1aa764ecdf0.jpg","https://i.pinimg.com/564x/0f/13/98/0f1398587ed44eb09a24daa0907368dd.jpg","https://i.pinimg.com/736x/65/31/9c/65319c674ebb6d68581855f4bab9c85d.jpg"];
    const image=ref(listImages[0])
    const handleClick = () => {
        image.value = listImages[Math.floor(Math.random() * listImages.length)];
    };
</script>

<style scoped>
img{
    width: 200px;
    height: 200px;
}
</style>