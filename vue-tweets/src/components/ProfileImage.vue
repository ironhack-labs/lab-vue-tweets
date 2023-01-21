<template>
    <img :src="tweet.user.image" alt="Profile picture" class="profile-picture"/>
</template>

<script setup>
const props = defineProps(["tweet"]);
</script>

<style scoped>

</style>