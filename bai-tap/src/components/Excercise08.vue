<template>
    <div>
        <h2>Bài 8</h2>
        <a @click.stop.prevent="checkLink" href="https://www.google.com">Link lỗi</a>
        <a @click.stop.prevent="checkLink" href="http://www.google.com">Link đúng</a>
    </div>
</template>

<script setup>
 const checkLink=(e)=>{
    const href=e.target.href;
    if(href.startsWith('https://')){
        alert('Đường dẫn không hợp lê')
    }else{
        window.location.href=href;
    }
 }
</script>

<style>

</style>