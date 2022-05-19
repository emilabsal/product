<template lang="pug">
.sphere.container 
  .sphere-desc 
    span.sphere-subtitle {{ sphere.subtitle }}
    h3.title.sphere-title {{ sphere.title }}
    .sphere-content 
      slot
  .sphere-image
    img(
      :src="require(`@/assets/image/sphere/${sphere.img}`)",
      :alt="sphere.title"
    )
</template>

<script>
export default {
  props: {
    sphere: Object,
  },
};
</script>

<style lang="sass" scoped>
.sphere
  display: flex
  align-items: center
  justify-content: space-between
  gap: 84px
  margin-bottom: 150px
  &-title
    margin-bottom: 23px
  &-subtitle
    margin-bottom: 8px
    +text($fz: 16px, $lh: 24px, $fw: 600)
</style>