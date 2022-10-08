<script setup>
  const story = await useStoryblok('home', {
    version: 'draft'
  })
</script>

<template>
  <div>
    <StoryblokComponent v-if="story" :blok="story.content"></StoryblokComponent>
  </div>
</template>
