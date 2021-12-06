<template>
  <div>
    <article>
      <h2>{{ post.title }}</h2>
      <p>{{ post.description }}</p>
      <nuxt-content class="text-xl leading-10 w-1/2" :document="post" />
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