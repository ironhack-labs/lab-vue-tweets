<template>
  <div class="app">
    <Tweet
      v-for="(tweet, index) in tweets"
      :key="index"
      :user="tweet.user"
      :timestamp="tweet.timestamp"
      :message="tweet.message"
    />
  </div>
</template>

<script>
import Tweet from "./components/Tweet.vue";

export default {
  components: {
    Tweet,
  },
  data: () => ({
    tweets: [
      {
        user: {
          name: "Thoughts of Dog®",
          image: "https://i.imgur.com/b0EdHVV.jpg",
          handle: "dog_feelings",
        },
        timestamp: "1h ago",
        message:
          "the human likes to say. that i live here rent free. but i would argue. this housing accommodation. is my payment. for a lifetime of love. and excellent company",
      },
      {
        user: {
          name: "Thoughts of Dog®",
          image: "https://i.imgur.com/b0EdHVV.jpg",
          handle: "dog_feelings",
        },
        timestamp: "2h ago",
        message:
          "sometimes. the human presses their noggin against mine. to figure out what i’m thinking. so i just think really hard. about how much i love them. and hope they figure it out",
      },
      {
        user: {
          name: "Thoughts of Dog®",
          image: "https://i.imgur.com/b0EdHVV.jpg",
          handle: "dog_feelings",
        },
        timestamp: "3h ago",
        message:
          "here is what. i plan to accomplish today: \n\n2. bark loudly. but at nothing \n7. lose my ball under the couch\n7b. politely ask the human. to get my ball\n3. immediately lose it again. under the same couch\n4. big nap. you have worked hard\n2. repeat",
      },
    ],
  }),
};
</script>

<style></style>
