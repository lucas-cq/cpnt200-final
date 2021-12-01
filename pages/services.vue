<template>
  <div>
    <Navigation/>
      <section class="flex justify-around flex-wrap mx-auto bg-indigo-light">
        <article class="mx-20 mb-40 mt-52">
          <h1 class="text-5xl mb-10 text-purple-med"><strong>Services</strong></h1>
          <p class="text-2xl tracking-wide leading-relaxed"> Our team specializes in a variety <br> of services to best suit <br> our customers needs</p>
        </article>
        <div class="img-box">
          <img src="assets/images/linechart.png" />
        </div>
      </section>
      <section class="bg-indigo-dark">
        <h2 class="text-center pt-20 text-4xl text-purple-med"><strong>What We Offer</strong></h2>
        <div class="service-box">
          <ServiceCard v-for="service in services" :key="service.id" :info="service" />
        </div>
      </section>
    <Footer/>
  </div>
</template>

<style lang="postcss">
.img-box {
  @apply w-96
}
.service-box {
  @apply flex justify-around flex-wrap mx-60
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