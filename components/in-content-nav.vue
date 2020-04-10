<template>
  <!-- In body nav -->
  <nav class="in-body">
    <ul>
      <li v-for="(item, index) in navItems" :key="index">
        <nuxt-link :to="item.path">{{item.text}}</nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'InContentNav',
  data: function() {
    return {
      navItems: [
        { path: '/about', text: 'About' },
        { path: '/resume', text: 'Resume' },
        { path: '/portfolio', text: 'Portfolio' },
        { path: '/contact', text: 'Contact' }
      ]
    }
  }
}
</script>

<style scoped>
ul {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  justify-items: center;
}

ul li a {
  text-decoration: none;
}
ul li a:hover {
  color: #ab5f41;
}
</style>