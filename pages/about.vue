<template>
    <div>
        <h2>About</h2>  
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse facere odit sed placeat. Eveniet, dolorum quae magnam officiis eius tempore?</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam, nostrum!</p>
        <div>{{ me }}</div>
        <div>{{ currency }}</div>
        
    </div>
</template>

<script setup>
    const { data: me } = await useFetch('/api/rocker?name=Suzy', {
        method: 'post',
        body: { age: 30 }
    })

    const { data: currency } = await useFetch('/api/currency/GBP')
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
  