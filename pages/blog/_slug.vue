<template>
  <div class="font-Poppins">
    <Navigation />
    <section class="flex justify-start flex-wrap mx-auto bg-indigo-light">
    <article class="mx-40 mb-40 mt-52">
      <h1 class="text-4xl underline">{{ post.title }}</h1>
      <h2 class="text-2xl">{{ post.description }}</h2>
      <nuxt-content class="text-xl" :document="post" />
    </article>
    </section>
    <Footer />
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