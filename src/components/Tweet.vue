<template>
  <div class="tweet">
    <ProfileImage :imageUrl="tweet.user.image" />
    <div class="body">
      <div class="top">
        <User :user="tweet.user"/>
        <TimeStamp :time="tweet.timestamp" />
      </div>
      <Message :message="tweet.message" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import Actions from './Actions.vue';
import Message from './Message.vue';
import ProfileImage from './ProfileImage.vue';
import TimeStamp from './TimeStamp.vue';
import User from './User.vue';

export default {
  name: 'Tweet',
  props: {
    tweet:{
      type: Object,
      required: true,
    }
  },
    components: { Actions, Message, ProfileImage, TimeStamp, User }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
