<template>
  <div class="process-process section-container">
    <div class="process-max-width max-content-container">
      <span class="process-text">{{ text }}</span>
      <h2 class="process-text01 heading2">
        <span>
          We use a simple three step process.
          <span v-html="rawmtas"></span>
        </span>
        <br />
        <span>Take a look.</span>
      </h2>
      <div class="process-step">
        <span class="process-text05">{{ text1 }}</span>
        <div class="process-container">
          <span class="process-text06">{{ text4 }}</span>
          <span class="process-text07">{{ text5 }}</span>
        </div>
      </div>
      <div class="process-step1">
        <span class="process-text08">{{ text2 }}</span>
        <div class="process-container1">
          <span class="process-text09">{{ text6 }}</span>
          <span class="process-text10">{{ text7 }}</span>
        </div>
      </div>
      <div class="process-step2">
        <span class="process-text11">{{ text3 }}</span>
        <div class="process-container2">
          <span class="process-text12">{{ text8 }}</span>
          <span class="process-text13">{{ text9 }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Process',
  props: {
    text4: {
      type: String,
      default: 'Finding the best idea',
    },
    text8: {
      type: String,
      default: 'Strong design execution',
    },
    text: {
      type: String,
      default: 'Our process',
    },
    text1: {
      type: String,
      default: '01',
    },
    text3: {
      type: String,
      default: '03',
    },
    text9: {
      type: String,
      default:
        'As a creative, using your professional judgement, you should begin filtering your various ideas and designs, retaining the strongest relevant material.',
    },
    text7: {
      type: String,
      default:
        'Brainstorming is a process of toiling and generating new ideas alone or by holding intensive group discussions between team members in a team.',
    },
    text2: {
      type: String,
      default: '02',
    },
    text5: {
      type: String,
      default:
        'There are countless businesses already in existence, so it’s very likely that you won’t be the first person to think of an idea or product. There are countless businesses already in existence, so it’s very likely that you won’t be the first person to think of an idea or product. ',
    },
    text6: {
      type: String,
      default: 'Intense Brain storming ',
    },
  },

  data() {
    return {
      rawmtas: ' ',
    }
  },
}
</script>

<style scoped>
.process-process {
  position: relative;
  background-color: var(--dl-color-scheme-lightblue);
}
.process-max-width {
  align-items: flex-start;
  flex-direction: column;
  justify-content: space-between;
}
.process-text {
  color: var(--dl-color-scheme-white);
  font-style: normal;
  text-align: center;
  font-weight: 700;
  margin-bottom: 4px;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}
.process-text01 {
  color: var(--dl-color-scheme-white);
  margin-bottom: var(--dl-space-space-fourunits);
}
.process-step {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  border-color: rgba(255, 255, 255, 0.2);
  border-width: 1px;
  margin-bottom: var(--dl-space-space-fourunits);
  flex-direction: row;
  padding-bottom: 53px;
  border-top-width: 0px;
  border-left-width: 0px;
  border-right-width: 0px;
  border-bottom-width: 1px;
}
.process-text05 {
  color: var(--dl-color-scheme-white);
  font-size: 64px;
  font-style: normal;
  font-weight: 500;
  line-height: 61px;
  margin-right: 180px;
}
.process-container {
  flex: 1;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.process-text06 {
  color: var(--dl-color-scheme-white);
  font-size: 24px;
  line-height: 31px;
  margin-bottom: var(--dl-space-space-unit);
}
.process-text07 {
  color: var(--dl-color-scheme-white80);
}
.process-step1 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  border-color: rgba(255, 255, 255, 0.2);
  border-width: 1px;
  margin-bottom: var(--dl-space-space-fourunits);
  flex-direction: row;
  padding-bottom: 53px;
  border-top-width: 0px;
  border-left-width: 0px;
  border-right-width: 0px;
  border-bottom-width: 1px;
}
.process-text08 {
  color: var(--dl-color-scheme-white);
  font-size: 64px;
  font-style: normal;
  font-weight: 500;
  line-height: 61px;
  margin-right: 180px;
}
.process-container1 {
  flex: 1;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.process-text09 {
  color: var(--dl-color-scheme-white);
  font-size: 24px;
  line-height: 31px;
  margin-bottom: var(--dl-space-space-unit);
}
.process-text10 {
  color: var(--dl-color-scheme-white80);
}
.process-step2 {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  border-color: rgba(255, 255, 255, 0.2);
  border-width: 1px;
  flex-direction: row;
  padding-bottom: 53px;
  border-top-width: 0px;
  border-left-width: 0px;
  border-right-width: 0px;
  border-bottom-width: 1px;
}
.process-text11 {
  color: var(--dl-color-scheme-white);
  font-size: 64px;
  font-style: normal;
  font-weight: 500;
  line-height: 61px;
  margin-right: 180px;
}
.process-container2 {
  flex: 1;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
}
.process-text12 {
  color: var(--dl-color-scheme-white);
  font-size: 24px;
  line-height: 31px;
  margin-bottom: var(--dl-space-space-unit);
}
.process-text13 {
  color: var(--dl-color-scheme-white80);
}
@media(max-width: 767px) {
  .process-text05 {
    margin-right: var(--dl-space-space-fourunits);
  }
  .process-text08 {
    margin-right: var(--dl-space-space-fourunits);
  }
  .process-text11 {
    margin-right: var(--dl-space-space-fourunits);
  }
}
@media(max-width: 479px) {
  .process-text05 {
    margin-right: var(--dl-space-space-twounits);
  }
  .process-text08 {
    margin-right: var(--dl-space-space-twounits);
  }
  .process-text11 {
    margin-right: var(--dl-space-space-twounits);
  }
}
</style>
