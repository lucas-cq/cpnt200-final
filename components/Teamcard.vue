<template>
  <figure>
    <nuxt-img :src="info.pic" />
      <h3>{{ info.member }}</h3>
      <figcaption>{{ info.role }}</figcaption>
  </figure>
</template>

<style scoped lang="postcss">

</style>

<script>
export default {
  props: ['info']
}
</script>