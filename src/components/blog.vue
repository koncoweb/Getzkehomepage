<template>
  <div class="blog-blog section-container">
    <div class="blog-max-width max-content-container">
      <span class="blog-text">{{ text }}</span>
      <h2 class="blog-text1 heading2">
        <span>Our latest articles and resources</span>
      </h2>
      <span class="blog-text3">
        <span>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
          tempor incididunt
          <span v-html="rawrfro"></span>
        </span>
        <br />
        <span>
          ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
          exercitation.
        </span>
      </span>
      <button class="blog-primary button-secondary button-lg button">
        {{ primary }}
      </button>
      <div class="blog-blog-cards-container">
        <blog-card rootClassName="blog-card-root-class-name"></blog-card>
        <blog-card
          text1="Aug 14, 2022"
          button="advertising"
          image_src="/playground_assets/rectangle%2099%20%5B1%5D-1500w.png"
          rootClassName="blog-card-root-class-name1"
        ></blog-card>
        <blog-card
          text1="Jul 12, 2022"
          button="Branding"
          image_src="/playground_assets/unsplash_h7qmwoxf6z8-1500w.png"
        ></blog-card>
      </div>
    </div>
  </div>
</template>

<script>
import BlogCard from './blog-card'

export default {
  name: 'Blog',
  props: {
    primary: {
      type: String,
      default: 'Explore the blog',
    },
    text: {
      type: String,
      default: 'from blog',
    },
  },
  components: {
    BlogCard,
  },

  data() {
    return {
      rawrfro: ' ',
    }
  },
}
</script>

<style scoped>
.blog-blog {
  position: relative;
}
.blog-max-width {
  align-items: center;
  flex-direction: column;
  justify-content: space-between;
}
.blog-text {
  color: var(--dl-color-scheme-brown);
  font-style: normal;
  text-align: center;
  font-weight: 700;
  margin-bottom: 4px;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}
.blog-text1 {
  text-align: center;
  margin-bottom: var(--dl-space-space-unit);
}
.blog-text3 {
  color: var(--dl-color-scheme-black80);
  text-align: center;
  line-height: 26px;
  margin-bottom: var(--dl-space-space-twounits);
}
.blog-primary {
  margin-bottom: var(--dl-space-space-threeunits);
}
.blog-blog-cards-container {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-between;
}
@media(max-width: 991px) {
  .blog-blog-cards-container {
    align-items: center;
    flex-direction: column;
  }
}
</style>
