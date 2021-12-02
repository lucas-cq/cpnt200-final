<template>
  <header class="absolute w-full">
    <nav class="container flex justify-between items-center py-4">
      <div>
        <nuxt-link to="/" class="font-bold text-4xl">Vexus</nuxt-link>
      </div>
      <ul class="flex gap-14 text-xl items-center">
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link to="/about">About</nuxt-link>
        <nuxt-link to="/blog">Blog</nuxt-link>
        <nuxt-link to="/services">Services</nuxt-link>
        <nuxt-link to="/contact" class="bg-purple-light px-4 py-1 rounded">Contact</nuxt-link>
      </ul>
    </nav>
  </header>
</template>
