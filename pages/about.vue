<template>
  <div>
    <!--Nav Here-->
    <section class="flex justify-around flex-wrap bg-indigo-light">
      <article class="m-20">
      <h1 class="text-5xl mb-10">About Us</h1>
        <p class="text-2xl tracking-wide leading-relaxed">We are a passion driven team looking to <br>make a difference
          in the web <br> development industry.
        </p>
      </article>
        <div class="img-box">
          <nuxt-img src="assets/images/clipboard.png" />
        </div>
    </section>
    <!--Footer Here-->
    <section class="bg-indigo-dark">
      <div class="team-box">
        <Teamcard v-for="team in teams" :key="team.id" :info="team" />
      </div>
    </section>
  </div>
</template>

<style scoped lang="postcss">
.img-box {
  @apply w-96
}
.team-box {

}
</style>

<script>
export default {
  data() {
    return {
      teams: [
        {
          member: "Lucas",
          role: "Backend Dev",
          pic: "assets/images/lucas-github.jpg"
        },
        {
          member: "Raj",
          role: "Frontend Dev",
          pic: "assets/images/raj-github.jpg"
        },
        {
          member: "David",
          role: "Designer",
          pic: "assets/images/david-github.jpg"
        },
        {
          member: "Jesse",
          role: "Content Manager",
          pic: "assets/images/jesse-github.png"
        }
      ]
    }
  }
}
</script>

