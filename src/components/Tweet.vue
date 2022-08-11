<template>
  <div className="tweet">
    <TweetImage :src="user.image" />

    <div className="body">
      <div className="top">
        <TweetUser :user="user" />
        <TweetTimestamp :timestamp="timestamp" />
      </div>

      <TweetMessage :message="message" />
      <TweetActions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import TweetImage from "./TweetImage.vue";
import TweetMessage from "./TweetMessage.vue";
import TweetUser from "./TweetUser.vue";
import TweetActions from "./TweetActions.vue";
import TweetTimestamp from "./TweetTimestamp.vue";

export default {
  name: "Tweet",
  components: {
    TweetImage,
    TweetUser,
    TweetMessage,
    TweetActions,
    TweetTimestamp,
  },
  props: {
    user: Object,
    timestamp: String,
    message: String,
  },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
