<template>
  <div class="font-Poppins">
    <Navigation />
    <section class="flex justify-start items-center flex-wrap bg-indigo-light">
    <article class="ml-40 mr-auto mb-40 mt-36">
      <h1 class="text-4xl underline mb-4">{{ post.title }}</h1>
      <h2 class="text-2xl mb-6">{{ post.description }}</h2>
      <nuxt-img :src="post.banner" height="600" />
      <nuxt-content class="text-xl leading-10 w-1/2 mt-8" :document="post" />
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