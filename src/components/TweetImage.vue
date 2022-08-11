<template>
  <img :src="src" className="profile" alt="profile" />
</template>

<script>
export default {
  name: "TweetImage",
  props: {
    src: String,
  },
};
</script>

<style></style>
