<template>
  <div className="tweet">

    <ProfileImage :user="user" />

    <div className="body">
      <div className="top">
        <User :user="user"/>
        <Timestamp />
      </div>
      <Message :message="message"/>

      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>

import ProfileImage from "../components/ProfileImage.vue"
import Message from "../components/Message.vue"
import Timestamp from "../components/Timestamp.vue"
import Actions from "../components/Actions.vue"
import User from "../components/User.vue"

export default({
  name: "Tweet",
  components: { ProfileImage, Message, Timestamp, Actions, User },
  data() {
    return{
    }
  },
  props: {
    user: Object,
    message: String,
  },
})
</script>


<style scoped>
a {
  color: #42b983;
}
</style>
