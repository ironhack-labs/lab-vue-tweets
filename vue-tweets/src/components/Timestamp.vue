<template>
    <div class="flex center">
        <p>{{tweet.timestamp}}</p>
    </div>

</template>

<script setup>
const props = defineProps(["tweet"]);

</script>

<style scoped>

</style>