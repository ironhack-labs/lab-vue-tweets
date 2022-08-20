<template>
    <img :src="imageUrl" className="profile" alt="profile" />
</template>

<script>
export default {
  name: 'ProfileImage',
  props: {
    imageUrl: String,
  },
}
</script>
