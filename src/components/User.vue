<template>
  <span className="user">
    <span className="name">{{ userData }}</span>
    <span className="handle">{{ userData }}</span>
  </span>
</template>

<script>

import TweetsArray from '../components/TweetsArray.vue';

export default {

  name: 'userData',
  
  components: {
    TweetsArray,
  },

  props: {
    userData: {
      required: true,
      type: Object,
    },
  },
  
};
</script>