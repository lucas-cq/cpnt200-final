<template>
  <div class="font-Poppins relative">
    <Navigation/>
    <main class="h-screen bg-indigo-light">
      <div class="container h-full flex justify-center items-center">
        <div class="w-1/2">
          <h1 class="font-bold text-6xl leading-normal mb-8">The Creative Agency<br>For <span class="text-purple-med">Innovative</span><br>Digital Experiences</h1>
          <nuxt-link to="/contact" class="bg-purple-light px-4 py-1 rounded text-xl">Let's Talk</nuxt-link>
        </div>
        <div>
          <nuxt-img src="/assets/images/computer.png" sizes="sm:100vw md:50vw lg:40vw"/>
        </div>
      </div>
    </main>

    <Footer/>
  </div>
</template>

<style lang="postcss">

</style>

<script>
export default {
   head() {
    return {
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },
}
</script>
