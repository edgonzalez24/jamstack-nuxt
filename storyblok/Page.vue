<script setup>
  defineProps({
    blok: Object
  });

</script>
<template>
  <div v-editable="blok">
    <StoryblokComponent
      v-for="item in blok.body"
      :key="item._uid"
      :blok="item"
    >

    </StoryblokComponent>
  </div>
</template>