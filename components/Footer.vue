<template>
  <footer class="bg-black">
    <div class="container flex justify-between items-center py-12 text-white">
      <div>
        <nuxt-link to="/" class="font-bold text-4xl">Vexus</nuxt-link>

      </div>

      <div class="flex flex-col gap-4">
        <h2 class="font-bold border-b-2 w-max">Contact Us</h2>
        <p>info@vexus.com</p>
        <p>(403) 888-8888 </p>
        <p>100 10th Ave SW</p>
      </div>

      <ul class="flex flex-col gap-4 text-xl items-center justify-center">
        <nuxt-link to="/about">About</nuxt-link>
        <nuxt-link to="/blog">Blog</nuxt-link>
        <nuxt-link to="/services">Services</nuxt-link>
      </ul>
    </div>
  </footer>
</template>

<style scoped lang="postcss">

</style>