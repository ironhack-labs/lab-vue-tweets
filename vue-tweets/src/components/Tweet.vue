<template>
    <div class="flex tweet">
        <ProfileImage :tweet="tweet"/>
        <div class="inner-tweet">
            <User :tweet="tweet"/>
            <div>
                <Message :tweet="tweet"/>
            </div>
            <Actions />
        </div>
    </div>
    
</template>

<script setup>
import { ref } from 'vue';
import ProfileImage from "./ProfileImage.vue"
import User from "./User.vue"
import Message from "./Message.vue"
import Actions from "./Actions.vue"
const props = defineProps(["tweet"]);

</script>

<style scoped>

</style>