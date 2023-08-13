<template>
    <div>
        <header>
            <nav>
                <NuxtLink to="/products">Nuxt Rocks! - Products</NuxtLink>
            </nav>
        </header>

        <!-- output the page content -->
        <div>
            <slot />
        </div>

        <footer>
            <ul>
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <li><NuxtLink to="/products">Products</NuxtLink></li>
            </ul>            
        </footer>
    </div>
</template>

<script setup>

</script>

<style scoped>
    .router-link-exact-active {
        color: #12b488;
    }
</style>
  