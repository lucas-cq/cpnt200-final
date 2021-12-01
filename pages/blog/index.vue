<template>
  <div class="font-Poppins">
    <Navigation />
    <main class="h-screen bg-indigo-light">
      <section class="container flex justify-between flex-wrap items-center h-full">
        <article class="w-1/2">
          <h1 class="text-6xl leading-normal text-purple-med"><strong>Articles</strong></h1>
          <p class="text-3xl leading-normal">A collection of our finest articles written by nerds <br>like you.</p>
        </article>
          <div>
            <nuxt-img src="assets/images/pencil-case.png" sizes="sm:100vw md:50vw lg:30vw" />
          </div>
      </section>
    </main>
    <div class="article-box">
        <div class="article-li" v-for="post in posts" :key="post.slug">
          <nuxt-link class="text-4xl hover:text-purple-med" :to="`blog/${post.slug}`">{{ post.title }}</nuxt-link>
          <p class="text-2xl pt-6">{{ post.description }}</p>
        </div>
      </div>
    <Footer />
  </div>
</template>

<style scoped lang="postcss">
.article-box {
  @apply bg-indigo-dark flex justify-center flex-col flex-wrap mx-auto
}

.article-li {
  @apply my-20 pl-64
}

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