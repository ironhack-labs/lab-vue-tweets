<template>
    <Tweet v-for="tweet in tweets" :tweet="tweet"/>
</template>

<script setup>
import Tweet from './components/Tweet.vue';
import { ref } from 'vue';

const tweets = ref ([{
    user: {
        name: "Thoughts of Cat®",
        image: "https://d.newsweek.com/en/full/1920025/cat-its-mouth-open.jpg?w=1600&h=1600&q=88&f=b7a44663e082b8041129616b6b73328d",
        handle: "cat_feelings",
    },
    timestamp: "1h ago",
    message: "the human likes to say. that i live here rent free. but i would argue. this housing accommodation. is my payment. for a lifetime of love. and excellent company",
  },
  {
    user: {
        name: "Thoughts of Cat®",
        image: "https://d.newsweek.com/en/full/1920025/cat-its-mouth-open.jpg?w=1600&h=1600&q=88&f=b7a44663e082b8041129616b6b73328d",
        handle: "cat_feelings",
    },
    timestamp: "2h ago",
    message: "sometimes. the human presses their noggin against mine. to figure out what i’m thinking. so i just think really hard. about how much i love them. and hope they figure it out",
  },
  {
    user: {
        name: "Thoughts of Cat®",
        image: "https://d.newsweek.com/en/full/1920025/cat-its-mouth-open.jpg?w=1600&h=1600&q=88&f=b7a44663e082b8041129616b6b73328d",
        handle: "cat_feelings",
    },
    timestamp: "3h ago",
    message: "here is what. i plan to accomplish today: \n\n2. bark loudly. but at nothing \n7. lose my ball under the couch\n7b. politely ask the human. to get my ball\n3. immediately lose it again. under the same couch\n4. big nap. you have worked hard\n2. repeat",
  }])

</script>

<style scoped>

</style>