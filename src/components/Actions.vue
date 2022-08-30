<template>
    <div className="actions">
      <i class="far fa-comment"></i>
      <i class="fas fa-retweet" @click="$emit('clickRetweet')"></i>
      <i class="fas" :class="isLikeHeart" @click="$emit('clickLike')"></i>
      <i class="fas fa-share"></i>
    </div>
</template>

<script>

export default {
    name : "Actions",
    props: {
        icon: Boolean,
        retweeted: Boolean,
    },
    computed: {//reactive
      isLikeHeart(){
        if(this.icon){
          return 'fa-solid fa-heart tweet-color';
        }else{
          return 'fa-regular fa-heart ';
        }
      }
    }
}
</script>

<style>
.tweet-color{
    color:tomato;
}
</style>