<template>
  <div class="font-Poppins relative">
    <Navigation />

    <main class="h-screen bg-indigo-light">
      <div class="container h-full flex justify-between items-center">
        <div class="w-1/2">
          <h1 class="font-bold text-6xl leading-normal text-purple-med">Lets Talk</h1>
          <p class="text-3xl leading-normal">We would love to hear from you! Please feel free to contact us about any questions you have or to set up a consultation with us.</p>
        </div>
        <div>
          <nuxt-img src="/assets/images/chatting.png" height="1000" width="500" sizes="sm:100vw md:50vw lg:50vw"/>
        </div>
      </div>
    </main>

    <section class="h-screen bg-indigo-dark flex flex-col items-center justify-center">
      <div>
        <h1 class="font-bold text-6xl leading-normal text-purple-med border-b-2 border-black w-max">Contact Us</h1>
      </div>

      <div class="flex gap-8 my-20">
        <div class="service-box">
          <h2 class="text-2xl font-bold">Location</h2>
          <p>100 10th Ave SW</p>
          <p>Calgary, Alberta</p>
        </div>
        <div class="service-box">
          <h2 class="text-2xl font-bold">Phone</h2>
          <p>(403) 888-8888</p>
        </div>
        <div class="service-box">
          <h2 class="text-2xl font-bold">Email</h2>
          <p>info@vexus.com</p>
        </div>
        <div class="service-box">
          <h2 class="text-2xl font-bold">Hours</h2>
          <p>Monday-Friday</p>
          <p>8am - 5pm</p>
        </div>
      </div>
    </section>

    <Footer />
  </div>
</template>

<style lang="postcss">
.service-box {
  @apply border-0 bg-indigo-light p-12 text-center flex flex-col gap-4 rounded-md
}
</style>