<template>
  <div>

    <!-- Navigation -->  
    <Navigation />

    <!-- Content -->
    <nuxt />

    <!-- Footer -->
    <PageFooter />

  </div>
</template>

<script>
import PageFooter from '../components/footer.vue'
import Navigation from '../components/navigation.vue'

export default {
  components: {
    PageFooter,
    Navigation,
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
  color: #ffffff;
  overflow-x: hidden;
}

.content-container {
  height: calc(100vh - 160px);
  display: grid;
  align-items: center;

}

a {
  color: #ffffff;
  text-transform: uppercase;
}

.inner {
  max-width: 1300px;
  margin: 15px auto;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
</style>
