<script setup>
const slug = useRoute().params.slug
const { data: post } = await useAsyncData(`blog-${slug}`, () => {
  return queryCollection('blog').path(`/blog/${slug}`).first()
})
const allPosts = await queryCollection('blog').order('title', 'DATE').all()
</script>

<template>
  <!-- Render the blog post as Prose & Vue components -->
   <NuxtPage />
  <ContentRenderer v-if="post" :value="post" />
</template>