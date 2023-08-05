<template>
    <div>
        <h2>Ravenclaw</h2>
        <div class="image">
            <img :src="'/ravenclaw.png'" width ="600" class="mx-auto">
        </div>
            <p> Intelligent and wise, they appreciate creativity and love of learning; their emblem is an eagle. </p>
        </div>
</template>

<script setup>

</script>

<style scoped>
    .image {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    h2 {
        margin-bottom:  20px;
        font-size: 36px;
    }
    p {
        text-align: center;
        margin: 20px 0;
    }
</style>