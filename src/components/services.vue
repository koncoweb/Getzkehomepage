<template>
  <div class="services-services section-container">
    <div class="services-max-width max-content-container">
      <div class="services-heading-container">
        <div class="services-text-container">
          <span class="services-text">{{ text }}</span>
          <h2 class="heading2">
            <span>
              We provide a wide range of
              <span v-html="rawov6t"></span>
            </span>
            <br />
            <span>creative solutions</span>
          </h2>
        </div>
        <div class="services-controls">
          <button class="control-btn">
            <svg viewBox="0 0 1024 1024" class="services-icon">
              <path
                d="M402.746 877.254l-320-320c-24.994-24.992-24.994-65.516 0-90.51l320-320c24.994-24.992 65.516-24.992 90.51 0 24.994 24.994 24.994 65.516 0 90.51l-210.746 210.746h613.49c35.346 0 64 28.654 64 64s-28.654 64-64 64h-613.49l210.746 210.746c12.496 12.496 18.744 28.876 18.744 45.254s-6.248 32.758-18.744 45.254c-24.994 24.994-65.516 24.994-90.51 0z"
              ></path>
            </svg>
            {{ button }}
          </button>
          <button class="control-btn">
            <svg viewBox="0 0 1024 1024" class="services-icon2">
              <path
                d="M621.254 877.254l320-320c24.994-24.992 24.994-65.516 0-90.51l-320-320c-24.994-24.992-65.516-24.992-90.51 0-24.994 24.994-24.994 65.516 0 90.51l210.746 210.746h-613.49c-35.346 0-64 28.654-64 64s28.654 64 64 64h613.49l-210.746 210.746c-12.496 12.496-18.744 28.876-18.744 45.254s6.248 32.758 18.744 45.254c24.994 24.994 65.516 24.994 90.51 0z"
              ></path>
            </svg>
            {{ button1 }}
          </button>
        </div>
      </div>
      <div class="services-cards-container">
        <services-card></services-card>
        <services-card
          text="Copy-writting"
          image_src="/playground_assets/file-document-200w.png"
        ></services-card>
        <services-card
          text="Product Design"
          image_src="/playground_assets/dice-5-200h.png"
        ></services-card>
      </div>
    </div>
  </div>
</template>

<script>
import ServicesCard from './services-card'

export default {
  name: 'Services',
  props: {
    button1: String,
    text: {
      type: String,
      default: 'our services',
    },
    button: String,
  },
  components: {
    ServicesCard,
  },

  data() {
    return {
      rawov6t: ' ',
    }
  },
}
</script>

<style scoped>
.services-services {
  display: flex;
  position: relative;
  padding-top: var(--dl-space-space-fiveunits);
  flex-direction: column;
  background-color: var(--dl-color-scheme-lightbrown);
}
.services-max-width {
  flex-direction: column;
}
.services-heading-container {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-end;
  margin-bottom: var(--dl-space-space-fourunits);
  flex-direction: row;
  justify-content: space-between;
}
.services-text-container {
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.services-text {
  color: var(--dl-color-scheme-brown);
  font-style: normal;
  text-align: center;
  font-weight: 700;
  margin-bottom: 4px;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}
.services-controls {
  display: grid;
  grid-gap: 12px;
  grid-template-columns: 1fr 1fr;
}
.services-icon {
  width: 16px;
  height: 16px;
}
.services-icon2 {
  width: 16px;
  height: 16px;
}
.services-cards-container {
  width: 100%;
  display: flex;
  grid-gap: 20px;
}
</style>
