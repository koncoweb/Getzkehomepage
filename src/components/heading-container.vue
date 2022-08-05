<template>
  <div class="heading-container-heading-container">
    <h1 class="heading-container-text heading1">
      <span>We are a creative agency based</span>
      <br />
      <span>in Massachusetts</span>
    </h1>
    <span class="heading-container-text3">
      <span>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
      </span>
      <br />
      <span>tempor incididunt ut labore et dolore magna aliqua.</span>
    </span>
    <button class="heading-container-primary button-primary button-lg button">
      {{ primary }}
    </button>
  </div>
</template>

<script>
export default {
  name: 'HeadingContainer',
  props: {
    primary: {
      type: String,
      default: 'Get in touch with us',
    },
  },
}
</script>

<style scoped>
.heading-container-heading-container {
  flex: 1;
  display: flex;
  position: relative;
  max-width: 100%;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.heading-container-text {
  text-align: center;
  margin-bottom: var(--dl-space-space-halfunit);
}
.heading-container-text3 {
  color: var(--dl-color-scheme-black);
  font-size: 18px;
  text-align: center;
  line-height: 1.44;
  margin-bottom: var(--dl-space-space-twounits);
}
.heading-container-primary {
  margin-bottom: var(--dl-space-space-threeunits);
}
@media(max-width: 991px) {
  .heading-container-heading-container {
    max-width: 100%;
    margin-bottom: 42px;
  }
}
@media(max-width: 767px) {
  .heading-container-text {
    font-size: 48px;
  }
}
</style>
