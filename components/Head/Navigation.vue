<template>
    <ul class="navigation">
        <li><NuxtLink v-if="isNotHome" to="/">Prima pagina</NuxtLink></li>
        <li>Pagina fata</li>
        <li>Urban</li>
        <li>Rural</li>
        <li>Politică</li>
        <li>Pagina spate</li>
    </ul>
</template>

<script setup lang="ts">
const route = useRoute()
const isNotHome = computed(() => route.fullPath !== '/')
</script>