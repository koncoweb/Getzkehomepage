<template>
  <div class="banner-banner section-container">
    <div class="banner-max-width max-content-container">
      <span class="banner-text">{{ text }}</span>
      <h2 class="banner-text1 heading2"><span>Let’s collaborate!</span></h2>
      <span class="banner-text3">
        <span>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
          tempor incididunt
          <span v-html="rawdv32"></span>
        </span>
        <br />
        <span>
          ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
          exercitation.
        </span>
      </span>
      <button class="banner-primary button-lg button-secondary-white button">
        {{ primary }}
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Banner',
  props: {
    primary: {
      type: String,
      default: 'Contact us',
    },
    text: {
      type: String,
      default: 'what are you waiting?',
    },
  },

  data() {
    return {
      rawdv32: ' ',
    }
  },
}
</script>

<style scoped>
.banner-banner {
  position: relative;
  background-color: var(--dl-color-scheme-brown);
}
.banner-max-width {
  align-items: center;
  flex-direction: column;
  justify-content: space-between;
}
.banner-text {
  color: var(--dl-color-scheme-white);
  font-style: normal;
  text-align: center;
  font-weight: 700;
  margin-bottom: 4px;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}
.banner-text1 {
  color: var(--dl-color-scheme-white);
  text-align: center;
  margin-bottom: var(--dl-space-space-unit);
}
.banner-text3 {
  color: var(--dl-color-scheme-white);
  text-align: center;
  line-height: 26px;
  margin-bottom: var(--dl-space-space-twounits);
}
.banner-primary {
  margin-bottom: var(--dl-space-space-threeunits);
}
</style>
