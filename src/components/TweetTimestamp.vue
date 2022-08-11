<template>
  <div>
    <span> {{ timestamp }} </span>
  </div>
</template>

<script>
export default {
  name: "TweetTimestamp",
  props: {
    timestamp: String,
  },
};
</script>

<style></style>
