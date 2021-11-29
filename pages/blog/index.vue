<template>
  <div class="font-Poppins">
    <Navigation />
    <section class="flex justify-around flex-wrap mx-auto bg-indigo-light">
      <article class="mx-20 mb-40 mt-52">
        <h1 class="text-5xl mb-10 text-purple-med"><strong>Articles</strong></h1>
        <p class="text-2xl tracking-wide leading-relaxed">A collection of our finest articles written by nerds <br>like you.</p>
      </article>
        <div class="img-box">
          <nuxt-img src="assets/images/pencil-case.png" />
        </div>
    </section>
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

.img-box {
  @apply w-96 mt-32
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