<template>
  <span class="user">
    <span class="name">{{ userData.name }}</span>
    <span class="handle">@{{ userData.handle }}</span>
  </span>
</template>

<script>
export default {
    props: {
        userData: Object,
    },
};
</script>
