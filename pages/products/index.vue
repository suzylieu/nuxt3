<template>
    <div>
        <h2>Products</h2>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products">
                <NuxtLink :to="`/products/${p.id}`">{{ p.title }}</NuxtLink>
            </div>
        </div>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Esse facere odit sed placeat. Eveniet, dolorum quae magnam officiis eius tempore?</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam, nostrum!</p>
    </div>
</template>

<script setup>
    definePageMeta({
        layout: 'products'
    })

    // fetch the products
    const { data: products } = await useFetch('https://fakestoreapi.com/products')
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
  