<template v-if="image">
  <img :src="image" className="profile" :alt="name" />
</template>

<script setup>
  defineProps({
    image: String,
    name: String,
  });
</script>

<style>
  
</style>