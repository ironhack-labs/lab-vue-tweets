<template>
    <span class="timestamp">{{time}}</span>
</template>

<script>
export default {
  name: 'TimeStamp',
  props: {
    time: {
        type: String,
        required: true
    }
  },
}
</script>
