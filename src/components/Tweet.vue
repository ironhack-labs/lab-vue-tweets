<template>
  <div className="tweet">
    <ProfileImage :src="user.image" />

    <div className="body">
      <div className="top">
        <User :user="user" />
        <Timestamp :timestamp="timestamp" />
      </div>

      <Message :message="message" />
      <Actions 
      :icon="icon"
      @clickLike="$emit('clickLike')"/>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>
<script>
  import Actions from "./Actions.vue";
  import Message from "./Message.vue";
  import User from "./User.vue";
  import Timestamp from "./Timestamp.vue";
  import ProfileImage from "./ProfileImage.vue";
  export  default {
    name : "Tweet",
    components :{
      Actions,
      User,
      Timestamp,
      Message,
      ProfileImage,
      
    },
    props:{
      user: Object,
      timestamp: String,
      message: String,
      icon: Boolean
    }
  }
</script>
<style scoped>
a {
  color: #42b983;
}
</style>
