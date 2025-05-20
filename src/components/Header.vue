<script setup>
    let num = Math.floor(Math.random() * 38) + 1;
    const logoheader = new URL(`../assets/header/LogoCesida-${num}.svg`, import.meta.url).href
</script>
<template>
    <header class="header">
        <img :src="logoheader" alt="Logotipo de Cesida">
    </header>
</template>
<style scoped>
    .header{
        background-color: #ffffff;
        position: fixed;
        right: 0;
        top: 0;
        width: calc(100vw - 20rem);
        height: 5rem;
        z-index: 999;
    }
    .header img{
        height: 1.5rem;
        position: absolute;
        right: 1.75rem;
        top: 50%;
        transform: translateY(-50%);
    }
</style>
