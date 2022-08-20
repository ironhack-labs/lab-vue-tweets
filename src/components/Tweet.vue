<template>
  <div className="tweet">
    <ProfileImage :image="user.image"/>

    <div className="body">
      <div className="top">
        <User :user="user"/>
        <Timestamp :timestamp="timestamp"/>
      </div>

      <p className="message">
        {{message}}
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
import ProfileImage from './ProfileImage.vue'
import User from './User.vue'
import Timestamp from "./Timestamp.vue";

export default {
  name: 'Tweet',
  components: {
    ProfileImage,
    User,
    Timestamp,
  },
  props: {
    user: {
      name: String,
      handle: String,
      image: String,
    },
    timestamp: String,
    message: String,
    },
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
