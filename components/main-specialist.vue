<template lang="pug">
.specialist
  img.specialst-image(
    :src="require(`@/assets/image/specialists/${spec.img}`)",
    alt=""
  )
  .specialist-block 
    p.text.specialist-text {{ spec.text }}
</template>

<script>
export default {
  props: ["spec"],
};
</script>

<style lang="sass" scoped>
.specialist
  display: flex
  align-items: center
  gap: 16px
  &:nth-child(2)
    flex-direction: row-reverse
  &:nth-child(3)
    flex-direction: row-reverse
  &-block
    border-radius: 27px
    padding: 15px 25px
    box-shadow: 0px 2px 8px rgba(86, 117, 146, 0.1)
    background-color: var(--white)
    position: relative
    &::after
      content: ''
      position: absolute
      bottom: -8.5px
      left: 32px
      width: 17px
      height: 17px
      border-radius: 50%
      background-color: var(--white)
      box-shadow: 0px 2px 8px rgba(86, 117, 146, 0.1)
</style>