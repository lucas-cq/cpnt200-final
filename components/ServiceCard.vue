<template>
  <section class="card-box">
    <div class="member-card">
      <h3 class="text-2xl text-center mt-4 mb-7">{{ info.title }}</h3>
      <p class="text-center text-lg">{{ info.text }}</p>
    </div >
  </section>
</template>

<style scoped lang="postcss">
  .card-box {
    @apply my-20 pb-16 pt-10 px-12 bg-indigo-light rounded-md
  }
</style>

<script>
export default {
  props: ['info']
}
</script>