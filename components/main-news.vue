<template lang="pug">
.news
  .news-inner.container
    h2.news-title Contents Strategies
    p.text.news-text We focus on ergonomics and meeting you where you work. It's only a keystroke away.
    swiper(ref="swiper", :options="swiperOptions") 
      swiper-slide.slide(v-for="(slide, index) in slides", :key="index")
        img.slide-img(
          :src="require(`@/assets/image/news/${slide.img}`)",
          :alt="slide.title"
        )
        .slide-desc
          p.slide-data By&nbsp;
            span.slide-author {{ slide.author }}
            | &nbsp; | &nbsp;
            span.slide-date {{ slide.date }}
          span.slide-title {{ slide.title }}
      .pagination(slot="pagination")
</template>

<script>
export default {
  data() {
    return {
      swiperOptions: {
        slidesPerView: 3,
        loop: true,
        spaceBetween: 32,
        pagination: {
          el: ".pagination",
          clickable: true,
          bulletClass: "pagination-dot",
          bulletActiveClass: "pagination-dot-active",
        },
      },
      slides: [
        {
          img: "news1.png",
          title: "Increasing Prosperity With Positive Thinking",
          author: "Wahid Ari",
          date: "03 March 2019",
        },
        {
          img: "news2.png",
          title: "Increasing Prosperity With Positive Thinking",
          author: "Wahid Ari",
          date: "03 March 2019",
        },
        {
          img: "news3.png",
          title: "Increasing Prosperity With Positive Thinking",
          author: "Wahid Ari",
          date: "03 March 2019",
        },
      ],
    };
  },
  computed: {
    swiper() {
      return this.$refs.swiper.$swiper;
    },
  },
};
</script>

<style lang="sass">
.news
  &-title
    +title($fz: 34px, $lh: 51px)
    margin-bottom: 8px
  &-text
    font-weight: 500
    margin-bottom: 33px

.slide
  border: 1px solid var(--grey)
  border-radius: 8px
  cursor: default
  overflow: hidden
  &-img
    max-width: 100%
    height: 185px
    object-fit: cover
    object-position: center
  &-desc
    padding: 24px
    padding-bottom: 40px
  &-data
    +text($fz: 16px, $lh: 28px, $fw: 400)
    margin-bottom: 12px
  &-author
    font-weight: 700
  &-title
    +title($fz: 24px, $lh: 40px)

.pagination
  margin-top: 64px
  display: flex
  align-items: center
  justify-content: center
  &-dot
    display: inline-block
    width: 16px
    height: 16px
    background-color: var(--grey)
    border-radius: 50%
    cursor: pointer
    margin: 0 5px
    &-active
      background-color: var(--green)
</style>