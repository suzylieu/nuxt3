<template>
    <div>
        <h2>Product details for {{ id }}</h2>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse facere odit sed placeat. Eveniet, dolorum quae magnam officiis eius tempore?</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam, nostrum!</p>
    </div>
</template>

<script setup>
    const { id } = useRoute().params

    definePageMeta({
        layout: 'products'
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
  