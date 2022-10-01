<template>
  <span className="user">
    <span className="name">{{ name }}</span>
    <span className="handle">{{ handle }}</span>
  </span>
</template>

<script setup>
  defineProps({
    name: String,
    handle: String
  })
</script>

<style>
  
</style>