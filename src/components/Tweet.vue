<template>
  <div className="tweet">
    <ProfileImage :image="tweet.user.image" />
    <div className="body">
      <User :user="tweet.user" :timestamp="tweet.timestamp" />

      <p className="message">{{ tweet.message }}</p>

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
export default {
  props: {
    tweet: Object,
  },
  components: { ProfileImage, User },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
