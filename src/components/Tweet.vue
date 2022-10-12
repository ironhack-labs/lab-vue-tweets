<template>
  <div className="tweet">
    <ProfileImage :src="tweet.user.image" />
    <div className="body">
      <div className="top">
      <User :userData="tweet.user.name" />
      <timestamp :timeStamp="tweet.timestamp" />
    </div>
      <Message :message="tweet.message"/>
      <Actions />
    </div>
  </div>
</template>

<script>

import Timestamp from './Timestamp.vue';
import User from './User.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';
import ProfileImage from './ProfileImage.vue';

export default {
  name: 'tweets',
  components: {
    User,
    Timestamp,
    Message,
    Actions,
    ProfileImage,
  },
  props:{
    tweet: {
      required: true,
      type: Object,
    },
  },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
