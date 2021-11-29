<template>
  <div class="font-Poppins">
    <Navigation/>
    <main>
      <div>
        <h1>The Creative Agency for <span>Innovative</span> Digital Experiences</h1>
        <nuxt-link to="/contact">Let's Talk</nuxt-link>
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
