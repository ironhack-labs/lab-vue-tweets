<template>
   <p className="message">
        {{ message }}
      </p>
</template>

<script>

export default {
  name: 'message',
  props: {
    message: {
      required: true,
      type: Object,
    },
  },
};
</script>