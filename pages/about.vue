<template>
  <div>
    <Navigation />
    <section class="flex justify-around flex-wrap mx-auto bg-indigo-light">
      <article class="mx-20 mb-40 mt-52">
      <h1 class="text-5xl mb-10 text-purple-med"><strong>About Us</strong></h1>
        <p class="text-2xl tracking-wide leading-relaxed">We are a passion driven team looking to <br>make a difference
          in the web <br> development industry.
        </p>
      </article>
        <div class="img-box">
          <nuxt-img src="assets/images/clipboard.png" />
        </div>
    </section>
    <section class="bg-indigo-dark">
      <h2 class="text-center pt-20 text-4xl text-purple-med"><strong>Our Team</strong></h2>
      <div class="team-box">
        <Teamcard v-for="team in teams" :key="team.id" :info="team" />
      </div>
    </section>
    <Footer />
  </div>
</template>

<style lang="postcss">
.img-box {
  @apply w-96 mt-32
}
.team-box {
  @apply flex justify-around flex-wrap mx-60
}
</style>

<script>
export default {
  data() {
    return {
      teams: [
        {
          member: "Lucas Cummings",
          role: "Backend Dev",
          pic: "assets/images/lucas-github.jpg"
        },
        {
          member: "Raj Hunjan",
          role: "Frontend Dev",
          pic: "assets/images/raj-github.jpg"
        },
        {
          member: "David Ha",
          role: "Designer",
          pic: "assets/images/david-github.jpg"
        },
        {
          member: "Jesse Thadi",
          role: "Content Manager",
          pic: "assets/images/jesse-github.png"
        }
      ]
    }
  }
}
</script>

