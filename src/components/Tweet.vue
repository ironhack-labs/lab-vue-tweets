<template>
  <div className="tweet">
    <ProfileImage :image="tweet.user.image" />
    <div className="body">
      <User :user="tweet.user" :timestamp="tweet.timestamp" />
      <Message :message="tweet.message" />

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
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Message from "./Message.vue";
export default {
  props: {
    tweet: Object,
  },
  components: { ProfileImage, User, Message },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
