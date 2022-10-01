<template>
  <span className="timestamp">{{ timestamp }}</span>
</template>

<script setup>
  defineProps({
    timestamp: String
  })
</script>