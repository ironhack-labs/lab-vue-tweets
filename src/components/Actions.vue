<template>
  <div className="actions">
    <!-- Font Awesome icons -->
    <i class="far fa-comment"></i>
    <i class="fas fa-retweet"></i>
    <i :class="likeStyle" @click="$emit('like')"></i>
    <i class="fas fa-share"></i>
  </div>
</template>

<script>
export default {
  props: {
    like: Boolean,
  },
  computed: {
    likeStyle() {
      if (this.like) {
        return "fa fa-heart red";
      } else {
        return "far fa-heart";
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
