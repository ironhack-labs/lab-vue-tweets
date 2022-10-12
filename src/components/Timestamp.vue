<template>
    <span className="timestamp">{{ timeStamp }}</span>
</template>

<script>

export default {
  name: 'timeStamp',
  props: {
    timeStamp: {
      required: true,
      type: Object,
    },
  },
  
};
</script>