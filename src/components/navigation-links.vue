<template>
  <nav class="navigation-links-nav" v-bind:class="rootClassName">
    <a href="https://getzke.id" class="navigation-links-link navigation-Link">
      {{ link1 }}
    </a>
    <a
      href="https://getzke.id/pesanan/"
      target="_blank"
      rel="noreferrer noopener"
      class="navigation-links-link1 navigation-Link"
    >
      {{ link2 }}
    </a>
    <a
      href="https://getzke.id/my-account/edit-account/"
      target="_blank"
      rel="noreferrer noopener"
      class="navigation-links-link2 navigation-Link"
    >
      {{ link3 }}
    </a>
  </nav>
</template>

<script>
export default {
  name: 'NavigationLinks',
  props: {
    link3: {
      type: String,
      default: 'Akun Anda',
    },
    rootClassName: String,
    link2: {
      type: String,
      default: 'Pesanan',
    },
    link1: {
      type: String,
      default: 'Home',
    },
  },
}
</script>

<style scoped>
.navigation-links-nav {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: row;
}
.navigation-links-link {
  color: #f9edd7;
  cursor: pointer;
  transition: 0.3s;
  text-decoration: none;
}
.navigation-links-link1 {
  color: #F9EDD7;
  cursor: pointer;
  transition: 0.3s;
  margin-left: 41px;
  text-decoration: none;
}
.navigation-links-link1:hover {
  color: var(--dl-color-scheme-brown);
}
.navigation-links-link2 {
  color: #F9EDD7;
  cursor: pointer;
  transition: 0.3s;
  margin-left: 41px;
  text-decoration: none;
}
.navigation-links-link2:hover {
  color: var(--dl-color-scheme-brown);
}








.navigation-links-root-class-name17 {
  margin-right: var(--dl-space-space-threeunits);
}
@media(max-width: 767px) {
  .navigation-links-nav {
    align-items: flex-start;
    flex-direction: column;
  }
  .navigation-links-link1 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-link2 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
}
</style>
