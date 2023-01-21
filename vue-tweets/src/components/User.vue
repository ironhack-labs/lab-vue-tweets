<template>
    <div class="flex center">
        <div class="flex user-details center">
            <h1>{{ tweet.user.name }}</h1>
            <p> @{{ tweet.user.handle }}</p>
            <p>·</p>
            <Timestamp :tweet="tweet"/>
        </div>
        <div class="flex plus-icon">
            <i class="fa-solid fa-ellipsis"></i> 
        </div>
    </div>

</template>

<script setup>
import Timestamp from "./Timestamp.vue";
const props = defineProps(["tweet"]);

</script>

<style scoped>

</style>