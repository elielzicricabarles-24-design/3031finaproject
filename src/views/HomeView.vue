<script setup>
import CoffeeSection from '@/sections/Home/CoffeeSection.vue'
import NonCoffeeSection from '@/sections/Home/NonCoffeeSection.vue'
</script>

<template>
    <div class="home-page">
        <CoffeeSection />
        <NonCoffeeSection />
    </div>
</template>

<style scoped>
.home-page {
    margin: 0px;
    width: 100%;
    min-height: 100vh;
    background-color: black;
}
</style>