<template>
  <div class="about-about section-container">
    <div class="about-max-width max-content-container">
      <div class="about-text-container">
        <span class="about-text">{{ text }}</span>
        <h2 class="about-text01 heading2">
          <span>
            We build brands with
            <span v-html="raw4b3l"></span>
          </span>
          <br />
          <span>purpose and impact</span>
        </h2>
        <span class="about-text05">{{ text1 }}</span>
        <div class="about-checklist">
          <div class="about-check-item">
            <svg viewBox="0 0 1024 1024" class="about-icon">
              <path d="M384 690l452-452 60 60-512 512-238-238 60-60z"></path>
            </svg>
            <span class="about-text06">{{ text2 }}</span>
          </div>
          <div class="about-check-item1">
            <svg viewBox="0 0 1024 1024" class="about-icon02">
              <path d="M384 690l452-452 60 60-512 512-238-238 60-60z"></path>
            </svg>
            <span class="about-text07">{{ text3 }}</span>
          </div>
          <div class="about-check-item2">
            <svg viewBox="0 0 1024 1024" class="about-icon04">
              <path d="M384 690l452-452 60 60-512 512-238-238 60-60z"></path>
            </svg>
            <span class="about-text08">{{ text4 }}</span>
          </div>
          <div class="about-check-item3">
            <svg viewBox="0 0 1024 1024" class="about-icon06">
              <path d="M384 690l452-452 60 60-512 512-238-238 60-60z"></path>
            </svg>
            <span class="about-text09">{{ text5 }}</span>
          </div>
          <div class="about-check-item4">
            <svg viewBox="0 0 1024 1024" class="about-icon08">
              <path d="M384 690l452-452 60 60-512 512-238-238 60-60z"></path>
            </svg>
            <span class="about-text10">{{ text6 }}</span>
          </div>
          <div class="about-check-item5">
            <svg viewBox="0 0 1024 1024" class="about-icon10">
              <path d="M384 690l452-452 60 60-512 512-238-238 60-60z"></path>
            </svg>
            <span class="about-text11">{{ text7 }}</span>
          </div>
        </div>
      </div>
      <div class="about-image-container">
        <img :alt="image_alt" :src="image_src" class="about-image" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'About',
  props: {
    text6: {
      type: String,
      default: 'Future-Proofing Projects',
    },
    text7: {
      type: String,
      default: 'Support in any implementation',
    },
    image_alt: {
      type: String,
      default: 'image',
    },
    text3: {
      type: String,
      default: 'Long-term strategy development',
    },
    image_src: {
      type: String,
      default: '/playground_assets/rectangle%20109-1000w.png',
    },
    text2: {
      type: String,
      default: 'Quality services and support all time',
    },
    text1: {
      type: String,
      default:
        'We are a full-service digital creative agency with brick and mortar offices and plenty of in-house talent.',
    },
    text: {
      type: String,
      default: 'about us',
    },
    text5: {
      type: String,
      default: 'Over 10 years in the business',
    },
    text4: {
      type: String,
      default: 'FREE Brand Audit for startups',
    },
  },

  data() {
    return {
      raw4b3l: ' ',
    }
  },
}
</script>

<style scoped>
.about-about {
  position: relative;
  background-color: var(--dl-color-scheme-lightbrown);
}
.about-max-width {
  flex-direction: row;
  justify-content: space-between;
}
.about-text-container {
  flex: 1;
  width: 40%;
  display: flex;
  align-items: flex-start;
  margin-right: var(--dl-space-space-unit);
  flex-direction: column;
}
.about-text {
  color: var(--dl-color-scheme-brown);
  font-style: normal;
  text-align: center;
  font-weight: 700;
  margin-bottom: 4px;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}
.about-text01 {
  margin-bottom: var(--dl-space-space-oneandhalfunits);
}
.about-text05 {
  color: var(--dl-color-scheme-black80);
  line-height: 26px;
  margin-bottom: var(--dl-space-space-twounits);
}
.about-checklist {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.about-check-item {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  margin-bottom: var(--dl-space-space-unit);
  flex-direction: row;
}
.about-icon {
  fill: var(--dl-color-scheme-brown);
  width: 18px;
  height: 18px;
  margin-right: var(--dl-space-space-unit);
}
.about-text06 {
  font-style: normal;
  font-weight: 500;
}
.about-check-item1 {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  margin-bottom: var(--dl-space-space-unit);
  flex-direction: row;
}
.about-icon02 {
  fill: var(--dl-color-scheme-brown);
  width: 18px;
  height: 18px;
  margin-right: var(--dl-space-space-unit);
}
.about-text07 {
  font-style: normal;
  font-weight: 500;
}
.about-check-item2 {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  margin-bottom: var(--dl-space-space-unit);
  flex-direction: row;
}
.about-icon04 {
  fill: var(--dl-color-scheme-brown);
  width: 18px;
  height: 18px;
  margin-right: var(--dl-space-space-unit);
}
.about-text08 {
  font-style: normal;
  font-weight: 500;
}
.about-check-item3 {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  margin-bottom: var(--dl-space-space-unit);
  flex-direction: row;
}
.about-icon06 {
  fill: var(--dl-color-scheme-brown);
  width: 18px;
  height: 18px;
  margin-right: var(--dl-space-space-unit);
}
.about-text09 {
  font-style: normal;
  font-weight: 500;
}
.about-check-item4 {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  margin-bottom: var(--dl-space-space-unit);
  flex-direction: row;
}
.about-icon08 {
  fill: var(--dl-color-scheme-brown);
  width: 18px;
  height: 18px;
  margin-right: var(--dl-space-space-unit);
}
.about-text10 {
  font-style: normal;
  font-weight: 500;
}
.about-check-item5 {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: row;
}
.about-icon10 {
  fill: var(--dl-color-scheme-brown);
  width: 18px;
  height: 18px;
  margin-right: var(--dl-space-space-unit);
}
.about-text11 {
  font-style: normal;
  font-weight: 500;
}
.about-image {
  flex: 1;
  object-fit: cover;
  border-radius: var(--dl-radius-radius-radius8);
}
@media(max-width: 991px) {
  .about-max-width {
    flex-direction: column;
  }
  .about-text-container {
    width: 100%;
    margin-right: 0px;
    margin-bottom: var(--dl-space-space-oneandhalfunits);
  }
  .about-image-container {
    width: 100%;
  }
  .about-image {
    width: 100%;
  }
}
</style>
