<template>
  <div className="tweet">
    <ProfileImage :image="image" />
    <div className="body">
      <div className="top">
        <span className="user">
          <User :user="user" />
        </span>

        <span className="timestamp">{{ timestamp }}</span>
      </div>

      <p className="message">
        {{ message }}
      </p>

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
    user: {
      name: String,
      handle: String,
    },
    timestamp: String,
    message: String,
    image: String,
  },
  components: { ProfileImage, User },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
