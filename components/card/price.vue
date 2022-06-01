<template lang="pug">
.card.cards
  span.card-title {{ price.title }}
  p.card-desc {{ price.desc }}
  .price
    span.price-num {{ price.price }}
    .price-desc 
      span.price-dollar $
      span.price-time Per / month
  ul.card-list
    li.card-item(v-for="(item, index) in price.list", :key="index") {{ item }}
  ui-button.card-button(title="Order Now")
</template>

<script>
export default {
  props: {
    price: "",
  },
};
</script>

<style lang="sass" scoped>
.card
  padding: 24px
  padding-bottom: 32px
  border-radius: 8px
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.25)
  display: flex
  flex-direction: column
  align-items: center
  flex-shrink: 0
  flex-grow: 1
  transition: .2s ease
  &:hover
    background-color: var(--green)
    *
      color: var(--white)
    .price-time
      color: #E0E0E0

  &-title
    +title($fz: 24px, $lh: 40px)
    margin-bottom: 8px
  &-desc
    +text($lh: 40px)
    margin-bottom: 16px
  &-list
    list-style-type: none
    margin-bottom: 38px
  &-item
    margin-bottom: 16px
    +text($lh: 22px, $fw: 500)
    text-align: center

.price
  display: flex
  align-items: center
  margin-bottom: 40px
  &-desc
    display: flex
    flex-direction: column
    align-items: flex-start

  &-num
    font-size: 71px
    line-height: 100px
    font-weight: 700
    color: var(--green)
    display: inline-block
    margin-right: 8px
  &-dollar
    font-size: 24px
    line-height: 30px
    font-weight: 700
    color: var(--green)
  &-time
    +text($lh: 19px)
    color: #AFAFAF
</style>