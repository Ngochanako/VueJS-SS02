<template>
     <div v-bind:class="elementClass" v-bind:id="elementId">
          Bài 2
     </div> 
</template>

<script setup>
let elementId='headingId';
let elementClass='headingClass'
</script>

<style scoped>
.headingClass{
    font-size: 24px;
    color: blue;
} 
#headingId{
    font-weight: bold;
    text-decoration: underline;
}
</style>