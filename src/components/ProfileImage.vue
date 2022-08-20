<template>
<img 
      :src="imageURL"
      className="profile"
      alt="profile"/>
</template>

<script>

export default {
  props: {   
    imageURL: String,
  },  
}
</script>