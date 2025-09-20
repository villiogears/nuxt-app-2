<script setup>
const slug = useRoute().params.slug
const { data: post } = await useAsyncData(`/${slug}`, () => {
  return queryCollection('/').path(`/${slug}`).first()
})
</script>

<template>
  <!-- Render the blog post as Prose & Vue components -->
  <ContentRenderer :value="post" />
</template>