<template lang="pug">
.feed
  .feed-stars 
    ui-icon(name="star-fill", v-for="index in feed.positive", :key="index")
    ui-icon(
      name="star-outline",
      v-for="index in 5 - feed.positive",
      :key="index"
    )
  p.feed-text {{ feed.text }}
  .feed-about
    img.feed-img(:src="require(`@/assets/image/feeds/${feed.img}`)", alt="")
    .feed-desc
      span.text.feed-name {{ feed.name }}
      span.feed-job {{ feed.job }}
</template>

<script>
export default {
  props: {
    feed: "",
  },
};
</script>

<style lang="sass" scoped>
.feed
  padding-top: 28px
  padding-left: 26px
  padding-right: 16px
  padding-bottom: 24px
  border-radius: 5px
  border: 1px solid var(--grey)
  &-text
    margin: 16px 0
    +text($lh: 28px)
    color: #737373
    letter-spacing: 0.2px
  &-about
    display: flex
    align-items: center
  &-img
    width: 50px
    height: 50px
    border-radius: 50%
    margin-right: 14px
  &-desc
    display: flex
    flex-direction: column
    justify-content: center
  &-name
    font-weight: 600
    color: var(--green)
    letter-spacing: 0.2px
  &-job
    +text($fz: 14px, $lh: 24px, $fw: 500)
    color: #252B42
    letter-spacing: 0.2px
</style>