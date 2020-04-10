<template>
  <div>
    <!-- Content -->
    <nuxt />

    <!-- Footer -->
    <page-footer />
  </div>
</template>

<script>
import PageFooter from '../components/footer.vue'

export default {
  components: {
    PageFooter
  }
}
</script>

<style>
html {
  font-family: 'Open Sans', sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

body {
  margin: 0;
  background-color: #24292e;
  color: #eff6ee;
}

a {
  color: #7ba19c;
}

.inner {
  max-width: 1300px;
  margin: 15px auto;
}
</style>
