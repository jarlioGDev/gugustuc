<template>
    <div class="pl-4 pr-4 text-justify">
        <NuxtLink :to="_path">
            <h1 class="text-4xl">
                {{ title }}
            </h1>
        </NuxtLink>
        <p class="pt-4 pb-4"> {{ description }}</p>
    </div>
</template>

<script setup>
const { content } = defineProps(['content']);
const { title, description, _path } = content;
</script>