<template>
    <p class="message">
        {{message}}
    </p>
</template>

<script>
export default {
  name: 'Message',
  props: {
    message: {
        type: String,
        required: true
    }
  },
}
</script>
