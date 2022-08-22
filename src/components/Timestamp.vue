<template>
    <span className="timestamp">{{ timeStamp }}</span>
</template>

<script>

import TweetsArray from '../components/TweetsArray.vue';

export default {

  name: 'timeStamp',
  
  components: {
    TweetsArray,
  },

  props: {
    timeStamp: {
      required: true,
      type: Object,
    },
  },
  
};
</script>