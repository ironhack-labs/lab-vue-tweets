<template>
  <img :src="image" className="profile" alt="profile" />
</template>

<script>
export default {
  props: {
    image: URL,
  },
};
</script>

<style></style>
