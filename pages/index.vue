<template>
    <div class="head-main-container">
        <HeadLogo />
        <div>
            <HeadText>Guguștucul</HeadText>
        </div>
    </div>
    <article class="article">
        <ArticleSummary v-for="article in articles" :content="article" :key="article.title" />
    </article>
</template>

<script setup>
const articles = await queryContent('/articles').find();
</script>