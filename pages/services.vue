<template>
<div>
    <Navigation/>
    <section class="flex justify-around flex-wrap mx-auto bg-indigo-light">
      <article class="m-20">
      <h1 class="text-5xl mb-10 text-purple-med"><strong>Services</strong></h1>
        <p class="text-2xl tracking-wide leading-relaxed">Something about our services
        </p>
      </article>
        <div class="img-box">
          <nuxt-img src="assets/images/linechart.png" />
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
      information: [
        {
         title: "",
         para: ""
        },
        {
         
        },
        {
          
        },
        {
          
        }
      ]
    }
  }
}
</script> 