<template>
     <div>
        <h2>Bài 7</h2>
        <form @submit.prevent="onsubmit" action="">
            <h4>Form</h4>
            <div style='display: flex;gap: 10px;'>
                <input type="text">
                <button type="submit">Submit</button>
            </div>
        </form>
     </div>
</template>

<script setup>
const onsubmit=(e)=>{
    console.log('Form submission prevented');   
}
</script>

<style>

</style>