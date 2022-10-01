<template>
  <div>
  <div className="tweet">
    <ProfileImage :image="tweet.user.image" :alt="tweet.user.name"  />

    <div className="body">
      <div className="top">
        <User :name="tweet.user.name" :handle="tweet.user.handle" />
        <Timestamp :timestamp="tweet.timestamp" />
      </div>

      <Message :message="tweet.message"/>
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</div>
</template>

<script setup>
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";

const props = defineProps({
  tweet: Object
})
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
