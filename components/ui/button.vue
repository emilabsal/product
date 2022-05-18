<template lang="pug">
button.button(v-if="!link", :class="outline ? 'outline' : icon ? 'icon' : ''")
  span.button-title(v-if="!icon") {{ title }}
  ui-icon.button-icon(v-if="icon", :name="name")
nuxt-link.button(
  v-else,
  :to="link",
  :class="outline ? 'outline' : icon ? 'icon' : ''"
) 
  span.button-title(v-if="!icon") {{ title }}
  ui-icon.button-icon(v-if="icon", :name="name")
</template>

<script>
export default {
  props: {
    link: String,
    icon: Boolean,
    name: String,
    title: String,
    outline: Boolean,
  },
};
</script>

<style lang="sass" scoped>
.button
  padding: 10px 24px
  background-color: $green
  cursor: pointer
  border: none
  outline: none
  border-radius: 4px
  &:hover,
  &-focus
    background-color: darken($green, 5%)

  &-title
    color: $white
    +text($lh: 24px, $fw: 600)

  &.outline
    background-color: transparent
    border: 1px solid $button-outline
    &:hover
      background-color: transparent
    .button-title
      color: $button-text

  &.icon
    padding: 0
    background-color: transparent
</style>
