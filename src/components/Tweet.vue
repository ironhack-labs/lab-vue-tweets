<template>
  <div className="tweet">
    <ProfileImage
      :image="user.image"
    ></ProfileImage>

    <div className="body">
      <div className="top">
        <User
          :username="user.name"
          :handle="user.handle"
        ></User>

        <Timestamp
          :timestamp="timestamp"
        ></Timestamp>
      </div>

      <Message
          :message="message"
      ></Message>

      <Actions/>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import User from './tweet/User.vue';
import Timestamp from './tweet/Timestamp.vue';
import ProfileImage from './tweet/ProfileImage.vue';
import Message from './tweet/Message.vue';
import Actions from './tweet/Actions.vue';

export default {
    components: {
    User,
    Timestamp,
    ProfileImage,
    Message,
    Actions
},
    props:['user', 'timestamp', 'message']
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
