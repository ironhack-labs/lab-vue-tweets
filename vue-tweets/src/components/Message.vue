<template>
    <p class="text-tweet">{{tweet.message}}</p>
</template>

<script setup>
const props = defineProps(["tweet"]);
</script>

<style scoped>

</style>