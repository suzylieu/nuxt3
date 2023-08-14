<template>
    <div>
        <h2>About</h2>  
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse facere odit sed placeat. Eveniet, dolorum quae magnam officiis eius tempore?</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam, nostrum!</p>
        <div>{{ data }}</div>
    </div>
</template>

<script setup>
    const { data } = await useFetch('/api/rocker?name=Suzy', {
        method: 'post',
        body: { age: 30 }
    })
</script>

<style scoped>
    h2 {
        margin-bottom: 20px;
        font-size: 36px;
    }
    p {
        margin: 20px 0;
    }
</style>
  