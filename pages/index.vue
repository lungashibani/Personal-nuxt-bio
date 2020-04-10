<template>
  <div class="inner">
    <!-- Header -->
    <header>
      <div>
        <h1>Lunga Shibani</h1>
      </div>

      <div class="slogan">Developer, QA Engineer, Creater</div>
    </header>
    <div class="content-container">
      <InContentNav />
    </div>
  </div>
</template>


<script>
import InContentNav from '../components/in-content-nav.vue'

export default {
  components: {
    InContentNav
  }
}
</script>

<style>
header {
  display: grid;
  padding: 10px;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  height: 20px;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

h1 {
  margin: 0;
  font-size: 28px;
}

.slogan {
  display: grid;
  justify-content: end;
}

.inner {
  text-decoration: none;
}

.inner .content-container {
  height: calc(100vh - 80px);
  display: grid;
  align-items: center;
  text-transform: uppercase;
  text-decoration: none;
}

a {
  color: #ffffff;
  text-transform: uppercase;
}
</style>>

