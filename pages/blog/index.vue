<template>
  <v-main>
    <h1>Articles</h1>
    <div v-for="post in posts" :key="post.slug">
      <nuxt-link :to="`blog/${post.slug}`">{{ post.title }}</nuxt-link>
    </div>
  </v-main>
</template>

<style scoped lang="postcss">

</style>

<script>
export default {
  async asyncData({ $content }) {
    const posts = await $content("blog").fetch();
    return {
      posts,
    };
  },
}
</script>