<template>
   <img
      :src="user.image"
      className="profile"
      alt="profile"
   />
</template>

<script>
export default {
   name: "ProfileImage",
   props: {
      user: Object,
   }
}
</script>

<style>

</style>