<template lang="pug">
header.header 
  .header-inner.container 
    nuxt-link(to="/")
      img(src="@/assets/image/logo.svg", alt="logo")
    .header-right 
      nav.nav 
        ul.nav-list 
          li.nav-item(v-for="(link, index) in links", :key="link") 
            nuxt-link.nav-link(:to="link.link") 
              | {{ link.title }}
      .sign
        ui-button(title="Sign In", :outline="true") 
        ui-button(title="Sign Up") 
        ui-button(:icon="true", name="theme") 
</template>

<script>
export default {
  data() {
    return {
      links: [
        { title: "Product", link: "/" },
        { title: "Customers", link: "/customers" },
        { title: "Prices", link: "/prices" },
        { title: "Resources", link: "/resources" },
      ],
    };
  },
};
</script>

<style lang="sass" scoped>
.header
  padding: 18px 0

  &-inner
    display: flex
    align-items: center
    justify-content: space-between
  &-right
    display: flex
    align-items: center

.nav
  margin-right: 24px
  &-list
    display: flex
    align-items: center
    list-style-type: none
  &-link
    display: inline-block
    text-decoration: none
    margin: 0 14px

.sign
  display: flex
  align-items: center
  gap: 24px

.nuxt-link-exact-active
  font-weight: 600
</style>