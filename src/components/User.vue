<template>
  <div className="top">
    <span className="user">
      <span className="name">{{ user.name }}</span>
      <span className="handle">{{ user.handle }}</span>
    </span>
    <span className="timestamp">{{ timestamp }}</span>
  </div>
</template>

<script>
export default {
  props: {
    user: Object,
    timestamp: String,
  },
};
</script>

<style></style>
