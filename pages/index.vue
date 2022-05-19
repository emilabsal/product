<template lang="pug">
main.main 
  .banner
    .banner-inner.container 
      .banner-desc 
        h1.banner-title Work at the speed of thought
        p.banner-text 
          | Tools, tutorials, design and innovation experts, all in one place! The most intuitive way to imagine your next user experience.
        .banner-buttons 
          ui-button.banner-button(title="Get started")
          ui-button.banner-button-secondary(
            title="Watch the Video",
            name="play",
            :withIcon="true"
          )
      .banner-img 
        img(src="@/assets/image/index/banner.svg", alt="banner")
  .advantages 
    .advantages-inner
      h2.title.advantages-title Product was Built Specifically for You
      .advantages-wrap 
        .advantages-overlay
        .advantages-block.container 
          .advantages-card(v-for="(adv, index) in advantages", :key="index") 
            ui-icon(:name="adv.name")
            span.advantages-card-title {{ adv.title }}
            p.text.advantages-card-text {{ adv.text }}
        ui-button.advantages-button(title="SING UP NOW")
  .spheres 
    main-sphere(
      v-for="(sphere, index) in spheres",
      :key="index",
      :sphere="sphere"
    )
      p.text.sphere-content-text 
        | The Myspace page defines the individual, his or her characteristics, traits, personal choices and the overall personality of the person.
      span.sphere-content-title Accessory makers
      p.text.sphere-content-text While most people enjoy casino gambling, sports betting, lottery and bingo playing for the fun
      span.sphere-content-title Alterationists
      p.text.sphere-content-text If you are looking for a new way to promote your business that won’t cost you more money,
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      advantages: [
        {
          name: "click",
          title: "First click tests",
          text: "While most people enjoy casino gambling,",
        },
        {
          name: "design",
          title: "Design surveys",
          text: "Sports betting, lottery and bingo playing for the fun",
        },
        {
          name: "preference",
          title: "Preference tests",
          text: "The Myspace page defines the individual.",
        },
        {
          name: "time",
          title: "Five second tests",
          text: "Personal choices and the overall personality of the person. ",
        },
      ],
      spheres: [
        {
          subtitle: "Effortless Validation for",
          title: "Management",
          img: "management.svg",
        },
      ],
    };
  },
};
</script>

<style lang="sass" scoped>
.banner
  margin-top: 25px
  &-inner
    display: flex
    align-items: center
    gap: 30px
  &-img
    max-width: 600px
  &-desc
    max-width: 480px
  &-title
    +title($fz: 40px, $lh: 60px)
    margin-bottom: 18px
  &-text
    +text($fz: 18px, $lh: 28px)
    margin-bottom: 45px
  &-buttons
    display: flex
    align-items: center
    gap: 30px
  &-button-secondary
    text-decoration: underline
    text-decoration-color: $green
    .button-title
      color: $green

.advantages
  margin-top: 114px
  margin-bottom: 149px
  &-title
    text-align: center
    margin-bottom: 58px
  &-block
    display: grid
    grid-template-columns: repeat(4, 1fr )
    justify-content: space-between
    gap: 46px
    margin-bottom: 60px
  &-wrap
    display: flex
    flex-direction: column
    align-items: center
    position: relative
  &-card
    svg
      margin-bottom: 30px
    &-title
      display: block
      +title($fz: 22px, $lh: 33px)
      margin-bottom: 13px
  &-overlay
    position: absolute
    bottom: 0
    left: -25%
    width: 150%
    height: 100%
    background: linear-gradient(179.59deg, #EDEDED 0.35%, rgba(255, 255, 255, 0.0001) 99.63%)
    z-index: -1
    transform: rotate(180deg)
    border-top-left-radius: 50%
    border-top-right-radius: 50%
  &-button
    margin-bottom: 90px

.sphere-content
  &-text
    margin-bottom: 30px
  &-title
    +text($fw: 600 )
    margin-bottom: 12px
</style>
