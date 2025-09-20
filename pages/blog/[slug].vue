<template>
    <NuxtPage />
    <ContentRenderer :value="post" />
</template>

<script setup>
const slug = useRoute().params.slug
const { data: post } = await useAsyncData(`blog-${slug}`, () => {
  return queryCollection('blog').path(`/${slug}`).first()
})
const allPosts = await queryCollection('blog').order('title', 'date').all()
</script>