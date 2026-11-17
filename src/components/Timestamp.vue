<template>
  <span class="timestamp">{{ time }}</span>
</template>

<script>
export default {
  name: "Timestamp",
  props: {
    time: String,
  },
};
</script>
