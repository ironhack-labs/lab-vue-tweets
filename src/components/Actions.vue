<template>
  <div className="actions">
    <!-- Font Awesome icons -->
    <i class="far fa-comment"></i>
    <i :class="retweetStyle" @click="$emit('retweet')"></i>
    <i :class="likeStyle" @click="$emit('like')"></i>
    <i class="fas fa-share"></i>
  </div>
</template>

<script>
export default {
  props: {
    like: Boolean,
    retweeted: Boolean,
  },
  computed: {
    likeStyle() {
      if (this.like) {
        return "fa fa-heart red";
      } else {
        return "far fa-heart";
      }
    },
    retweetStyle() {
      if (this.retweeted) {
        return "fas fa-retweet main-blue";
      } else {
        return "fas fa-retweet";
      }
    },
  },
};
</script>

<style scoped>
.red {
  color: red;
}
</style>
