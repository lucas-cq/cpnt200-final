<template>
  <div class="font-Poppins relative">
    <Navigation/>
      <section class="bg-indigo-light h-screen">
        <div class="container h-full flex justify-between items-center">
          <article class="w-1/2">
            <h1 class="font-bold text-6xl leading-normal text-purple-med">Services</h1>
            <p class="text-3xl leading-normal"> Our team specializes in a variety of services to best suit our customers needs</p>
          </article>
          <div>
            <img src="assets/images/linechart.png" width="750" />
          </div>
        </div>
      </section>
      <section class="bg-indigo-dark flex flex-col items-center justify-center py-8">
        <h2 class="font-bold text-6xl leading-normal text-purple-med border-b-2 border-black w-max">What We Offer</h2>
        <div class="container flex flex-wrap lg:flex-nowrap gap-8">
          <ServiceCard class="service-box" v-for="service in services" :key="service.id" :info="service" />
        </div>
      </section>
    <Footer/>
  </div>
</template>

<style lang="postcss">
.service-box {
  @apply border-0 bg-indigo-light p-12 text-center flex flex-col gap-4 rounded-md
}
</style>

<script>
export default {
  data() {
    return {
      services: [
        {
         title: "UX/UI design",
         text: "We have excellent UX/UI designs so that you have a website you're proud to show off"
        },
        {
         title: "Backend Development",
         text: "Amazing backend development to ensure you're website has the best performance"
        },
        {
         title: "Graphic Design",
         text: "We have great graphic design for your wonderful website"
        },
        {
         title: "SEO",
         text: "We'll make sure that your website is ranked up top with other websites and is user friendly"
        }
      ]
    }
  }
}
</script> 