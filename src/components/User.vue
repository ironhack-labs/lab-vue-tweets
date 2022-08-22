<template>
  <span className="user">
    <span className="name">{{ userData }}</span>
    <span className="handle">{{ userData }}</span>
  </span>
</template>

<script>

export default {

  name: 'userData',

  props: {
    userData: {
      required: true,
      type: Object,
    },
  },
  
};
</script>