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

    <section class="h-screen bg-indigo-dark">
      <div>
        <h1 class="font-bold text-6xl leading-normal text-purple-med border-b-2 border-black w-1/4">Contact Us</h1>
      </div>
    </section>

    <Footer />
  </div>
</template>