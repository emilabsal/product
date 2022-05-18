<template lang="pug">
header.header 
  .header-inner.container 
    nuxt-link(to="/")
      img(src="@/assets/image/logo.svg", alt="logo")
    .header-right 
      nav.nav 
        ul.nav-list 
          li.nav-item 
            nuxt-link.nav-link(to="/") 
              | Product
          li.nav-item 
            nuxt-link.nav-link(to="/") 
              | Customers
          li.nav-item 
            nuxt-link.nav-link(to="/") 
              | Prices
          li.nav-item 
            nuxt-link.nav-link(to="/") 
              | Resources
    .sign
      ui-button(title="Sign In", :outline="true") 
      ui-button(title="Sign Up") 
      ui-button(:icon="true", name="theme") 
</template>

<script>
export default {};
</script>

<style lang="sass" scoped>
</style>