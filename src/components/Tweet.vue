<template>
  <div className="tweet">
    <img
      src="https://i.imgur.com/9yw1Fyw.jpg"
      className="profile"
      alt="profile"
    />
    <div className="body">
      <div className="top">
      <User :userData="tweet.user.name" />
      <timestamp :timeStamp="tweet.timestamp" />
    </div>
      <Message :message="tweet.message"/>

      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>

import Timestamp from './Timestamp.vue';
import User from './User.vue';
import Message from './Message.vue';


export default {
  name: 'tweets',
  components: {
    User,
    Timestamp,
    Message,
  },
  props:{
    tweet: {
      required: true,
      type: Object,
    },
    userData: {
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
