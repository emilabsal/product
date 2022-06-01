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
        ui-button.advantages-button(title="SIGN UP NOW")
  .spheres 
    main-sphere.spheres-card(:sphere="spheres[0]")
      p.text.sphere-content-text 
        | The Myspace page defines the individual, his or her characteristics, traits, personal choices and the overall personality of the person.
      span.sphere-content-title Accessory makers
      p.text.sphere-content-text While most people enjoy casino gambling, sports betting, lottery and bingo playing for the fun
      span.sphere-content-title Alterationists
      p.text.sphere-content-text If you are looking for a new way to promote your business that won’t cost you more money,
    main-sphere.spheres-card(:sphere="spheres[1]")
      p.text.sphere-content-text The Myspace page defines the individual, his or her characteristics, traits, personal choices and the overall personality of the person.
      ul.sphere-content-list
        li.sphere-content-item 
          .sphere-content-icon 
            ui-icon(name="check")
          | Never worry about overpaying for your energy again.
        li.sphere-content-item 
          .sphere-content-icon 
            ui-icon(name="check")
          | We will only switch you to energy companies that we trust and will treat you right
        li.sphere-content-item 
          .sphere-content-icon 
            ui-icon(name="check")
          | We track the markets daily and know where the savings are.
    main-sphere.spheres-card(:sphere="spheres[2]")
      p.text.sphere-content-text 
        | Few would argue that, despite the advancements of feminism over the past three decades, women still face a double standard when it comes to their behavior.
      span.sphere-content-title Accessory makers
      p.text.sphere-content-text While most people enjoy casino gambling, sports betting, lottery and bingo playing for the fun
      span.sphere-content-title Alterationists
      p.text.sphere-content-text If you are looking for a new way to promote your business that won't cost you more money,
  .process
    .process-overlay
    h2.title.process-title Quick & Easy Process
    p.text.process-text Do you require some help for your project: Conception workshop, prototyping, marketing strategy, landing page, Ux/UI?
    .process-specialists.container
      main-specialist(
        v-for="(spec, index) in specialists",
        :key="index",
        :spec="spec"
      )
    ui-button(title="Contact our expert")
  main-news
  .price
    .price-inner.container
      h2.price-title Price Table
      p.text.price-text We offer competitive price
      .prices
        card-price(
          v-for="(price, index) in prices",
          :key="index",
          :price="price"
        )
  .feed
    .feed-inner.container
      h2.title.feed-title What Clients Say
      p.feed-subtitle Problems trying to resolve the conflict between the two major realms of Classical physics: Newtonian mechanics
      .feed-block
        card-feed(v-for="(feed, index) in feeds", :key="index", :feed="feed")
  .join
    .join-card
      .join-desc
        p.join-text Join 100 Compannies who boost their business with Product
        ui-button.secondary(title="Get This")
      img(src="@/assets/image/join.png", alt="")
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
        {
          subtitle: "Easier decision making for",
          title: "Customer Support",
          img: "support.svg",
        },
        {
          subtitle: "Optimisation for",
          title: "Collaborative",
          img: "management.svg",
        },
      ],
      specialists: [
        { img: "spec1.png", text: "I can take care of your pitch" },
        { img: "spec2.png", text: "I can take care of your pitch" },
        { img: "spec3.png", text: "I can take care of your pitch" },
        { img: "spec4.png", text: "I can take care of your pitch" },
      ],
      prices: [
        {
          title: "Free",
          desc: "Brief price description",
          price: 0,
          list: ["Only 2 Operators", "Notifications", "Landing Pages"],
        },
        {
          title: "Standard",
          desc: "Brief price description",
          price: 5,
          list: ["5+ Operators", "Notifications", "Landing Pages"],
        },
        {
          title: "Premium",
          desc: "Brief price description",
          price: 10,
          list: ["10+ Operators", "Notifications", "Landing Pages"],
        },
      ],
      feeds: [
        {
          positive: 5,
          text: "Product helps you see how many more days you need to work to reach your financial goal.",
          img: "client1.png",
          name: "Wahid Ari",
          job: "Designer",
        },
        {
          positive: 4,
          text: "Product helps you see how many more days you need to work to reach your financial goal.",
          img: "client1.png",
          name: "Wahid Ari",
          job: "Designer",
        },
        {
          positive: 4,
          text: "Product helps you see how many more days you need to work to reach your financial goal.",
          img: "client1.png",
          name: "Wahid Ari",
          job: "Designer",
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
    text-decoration-color: var(--green)
    .button-title
      color: var(--green)

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
  &-list
    list-style-type: none
  &-item
    display: flex
    align-items: center
    &:not(:last-child)
      margin-bottom: 30px
    &:nth-child(2) .sphere-content-icon
      background-color: var(--red)
    &:nth-child(3) .sphere-content-icon
      background-color: var(--blue)
  &-icon
    width: 35px
    height: 35px
    border-radius: 14px
    display: flex
    align-items: center
    justify-content: center
    background-color: var(--orange)
    flex-shrink: 0
    margin-right: 30px

.spheres
  &-card
    &:nth-child(2n)
      flex-direction: row-reverse

.process
  display: flex
  flex-direction: column
  align-items: center
  margin-bottom: 150px
  position: relative
  padding-top: 52px
  &::after
    content: ''
    position: absolute
    top: 0
    left: -20%
    width: 140%
    height: 100%
    background: linear-gradient(179.59deg, #EDEDED 0.35%, rgba(255, 255, 255, 0.0001) 99.63%)
    z-index: -1
    border-top-left-radius: 50%
    border-top-right-radius: 50%
  &-title
    margin-bottom: 16px
  &-text
    max-width: 542px
    text-align: center
    font-weight: 500
    margin-bottom: 32px
  &-specialists
    width: 100%
    display: grid
    grid-template-columns: repeat(2, 1fr)
    row-gap: 24px
    justify-content: space-between
    justify-items: start
    margin-bottom: 48px

.price
  margin-top: 150px
  margin-bottom: 150px
  &-title
    text-align: center
    +title($fz: 34px, $lh: 51px)
    margin-bottom: 8px
  &-text
    text-align: center
    font-weight: 500
    margin-bottom: 50px

.prices
  display: flex
  align-items: center
  gap: 71px

.feed
  &-title
    +title($lh: 57px)
    margin-bottom: 8px
    text-align: center
  &-subtitle
    text-align: center
    max-width: 537px
    margin: 0 auto
    margin-bottom: 50px
    font-weight: 500
  &-block
    display: flex
    gap: 20px
    justify-content: space-between

.join
  max-width: 968px
  background-color: var(--green)
  border-radius: 32px
  margin: 0 auto
  margin-top: 150px
  margin-bottom: 150px
  &-card
    display: flex
    align-items: center
  &-desc
    margin-left: 51px
  &-text
    font-size: 32px
    line-height: 151%
    font-weight: 600
    color: var(--white)
    margin-bottom: 46px
</style>
