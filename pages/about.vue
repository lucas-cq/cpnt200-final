<template>
  <div class="font-Poppins">
    <Navigation />
    <section class="bg-indigo-light h-screen">
      <div class="container flex justify-between items-center flex-wrap h-full">
        <article class="w-1/2">
        <h1 class="text-6xl leading-normal text-purple-med"><strong>About Us</strong></h1>
          <p class="text-3xl leading-normal">We are a passion driven team looking to make a difference
            in the web development industry.
          </p>
        </article>
          <div>
            <nuxt-img src="assets/images/clipboard.png" sizes="sm:100vw md:50vw lg:30vw" />
          </div>
      </div>
    </section>
    <section class="bg-indigo-dark h-screen">
      <div class="flex flex-col items-center justify-center gap-8">
        <h2 class="text-center pt-20 text-6xl text-purple-med border-b-2 border-black w-max"><strong>Our Team</strong></h2>
        <div class="team-box">
          <Teamcard v-for="team in teams" :key="team.id" :info="team" />
        </div>
      </div>
    </section>
    <Footer />
  </div>
</template>

<style lang="postcss">
.team-box {
  @apply flex justify-around flex-wrap mx-60 gap-8
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

