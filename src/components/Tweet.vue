<template>
  <div className="tweet">
    <profileImage 
      :imageURL="user.image">
    </profileImage>
    <div className="body">
      <div className="top">
        <user :user="user">
        </user>
        <timestamp :timestamp="timestamp">
        </timestamp>
      </div>

    <message :message="message"></message>
    <actions/>  

    
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>
<script>
import profileImage from './ProfileImage.vue';
import user from './User.vue';
import timestamp from './Timestamp.vue';
import message from './Message.vue';
import actions from './Actions.vue';

export default {
  props: {   
    user: {
      name: String,    
      handle: String,
      image: String,
    },
      timestamp:String,
      message:String,
  },
  components: {profileImage, user, timestamp,message, actions},
}
</script>
<style scoped>
a {
  color: #42b983;
}
</style>
