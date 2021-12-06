<template>
  <div>
    <article>
      <h2>{{ post.title }}</h2>
      <p>{{ post.description }}</p>
      <nuxt-img :src="post.banner" height="600" />
      <nuxt-content :document="post" />
    </article>
  </div>
</template>

<style lang="postcss">

</style>

<script>
export default {
  async asyncData({ $content, params, error }) {
    try {
      const post = await $content(`blog/${params.slug}`).fetch()
      return {
        post,
      }
    } catch (error) {
      error('No article found')
    }
  }
}
</script>