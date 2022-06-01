<template lang="pug">
button.button(
  @click="$emit('button-click')",
  v-if="!link",
  :class="(outline ? 'outline' : '') + (icon ? 'icon' : '') + (withIcon ? 'with-icon' : '')"
)
  ui-icon.button-icon(v-if="icon || withIcon", :name="name")
  span.button-title(v-if="title") {{ title }}
nuxt-link.button(
  v-else,
  :to="link",
  :class="(outline ? 'outline' : '') + (icon ? 'icon' : '') + (withIcon ? 'with-icon' : '')"
) 
  ui-icon.button-icon(v-if="icon", :name="name")
  span.button-title(v-if="!icon") {{ title }}
</template>

<script>
export default {
  props: {
    link: String,
    icon: Boolean,
    name: String,
    title: String,
    withIcon: Boolean,
    outline: Boolean,
  },
};
</script>

<style lang="sass" scoped>
.button
  padding: 10px 24px
  background-color: var(--green)
  cursor: pointer
  border: none
  outline: none
  border-radius: 4px
  &:hover,
  &:focus
    background-color: darken(#02897A, 5%)

  &-title
    color: var(--white)
    +text($lh: 24px, $fw: 600)

  &.outline
    background-color: transparent
    border: 1px solid var(--button-outline)
    &:hover
      background-color: transparent
    .button-title
      color: var(--button-text)

  &.icon
    padding: 0
    background-color: transparent

  &.with-icon
    background-color: transparent
    padding: 0
    display: flex
    align-items: center
    .button-title
      color: var(--green)
      margin-left: 8px
  &.secondary
    background-color: var(--white)
    .button-title
      color: var(--green)
.cards:hover
  .button
    background-color: var(--white)
  .button-title
    color: var(--green)
</style>
