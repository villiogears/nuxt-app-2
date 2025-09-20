<template>
    <NuxtPage />
    <ContentRenderer :value="post" />
</template>

<script setup>
const slug = useRoute().params.slug
const { data: post } = await useAsyncData(`blog-${slug}`, () => {
  return queryCollection('blog').path(`/${slug}`).first()
})
</script>