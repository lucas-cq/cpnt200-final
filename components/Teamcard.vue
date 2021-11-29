<template>
  <div class="member-box">
  <figure class="member-card">
    <nuxt-img class="w-40 rounded-full" :src="info.pic" />
      <h3 class="text-xl text-center mt-4">{{ info.member }}</h3>
      <figcaption class="text-center text-lg">{{ info.role }}</figcaption>
  </figure>
  </div>
</template>

<style scoped lang="postcss">
  .member-box {
    @apply my-20 pb-16 pt-10 px-12 bg-indigo-light rounded-md
  }
</style>

<script>
export default {
  props: ['info']
}
</script>