<template lang="pug">
footer.footer 
  .footer-inner.container
    .footer-col
      nuxt-link.logo(to="/")
        img.logo-img(src="@/assets/image/logo.svg", alt="logo")
      .social 
        a.social-icon(href="") 
          ui-icon(name="instagram")
        a.social-icon(href="")
          ui-icon(name="facebook")
        a.social-icon(href="")
          ui-icon(name="twitter")
    .footer-col 
      span.footer-title Resource
      nav.nav 
        ul.nav-list 
          li.nav-item 
            nuxt-link.nav-link(to="/")
              | About Us
          li.nav-item 
            nuxt-link.nav-link(to="/")
              | Blog
          li.nav-item 
            nuxt-link.nav-link(to="/")
              | Contact
          li.nav-item 
            nuxt-link.nav-link(to="/")
              | FAQ
    .footer-col 
      span.footer-title Legal Stuff
      nav.nav 
        ul.nav-list 
          li.nav-item 
            nuxt-link.nav-link(to="/")
              | Disclaimer
          li.nav-item 
            nuxt-link.nav-link(to="/")
              | Financing
          li.nav-item 
            nuxt-link.nav-link(to="/")
              | Privacy Policy
          li.nav-item 
            nuxt-link.nav-link(to="/")
              | Terms of Service
    .footer-col 
      span.footer-title knowing you're always on the best energy deal.
      form.form(action="")
        input.form-input(type="email")
        ui-button.form-button(title="Sign up Now") 
</template>

<script>
export default {};
</script>

<style lang="sass" scoped>
.footer
  padding: 46px 0
  margin-top: auto
  &-inner
    display: grid
    grid-template-columns: repeat(4, auto)
    gap: 20px
    justify-content: space-between
  &-title
    display: inline-block
    +text($fz: 20px, $lh: 30px, $fw: 500)
    margin-bottom: 8px
  &-col:last-child
    max-width: 325px

.logo
  display: inline-block
  margin-bottom: 24px
  &-img
    width: 163px

.social
  display: flex
  align-items: center
  gap: 16px
  &-icon
    width: 40px
    height: 40px
    border-radius: 50%
    display: flex
    align-items: center
    justify-content: center
    flex-shrink: 0
    background-color: var(--social)

.nav
  &-list
    list-style-type: none
  &-item
    margin-bottom: 8px
  &-link
    text-decoration: none

.form
  margin-top: 26px
  &-input
    display: block
    border: 1px solid var(--button-outline)
    outline: none
    padding: 10px 5px
    width: 100%
    margin-bottom: 21px
    filter: drop-shadow(0px 1px 2px rgba(0, 0, 0, 0.25))
    border-radius: 4px
    +text()
</style>