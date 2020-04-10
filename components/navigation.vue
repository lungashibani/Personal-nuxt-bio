<template>
  <header class="global-navigation">
    <!-- Home Link -->
    <div class="/">
      <nuxt-link to="/">LS</nuxt-link>
    </div>

    <!-- Menu -->
    <nav class="global-navigation_menu">
      <ul>
        <li v-for="(item, index) in navItems" :key="index">
          <nuxt-link :to="item.path">{{item.text}}</nuxt-link>
        </li>
      </ul>
    </nav>

    <!-- Contact -->
    <div class="global-navigation_contact">
      <nuxt-link to="/contact">Contact</nuxt-link>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Navigation',
  data: function() {
    return {
      navItems: [
        { path: '/about', text: 'About' },
        { path: '/resume', text: 'Resume' },
        { path: '/portfolio', text: 'Portfolio' }
        // { path: '/contact', text: 'Contact' }
      ]
    }
  }
}
</script>

<style scoped>
.global-navigation {
  height: 80px;
  background-color: #24292e;
  display: grid;
  grid-template: 'nav-home nav-menu nav-contact' 1fr / 80px 1fr 1fr;
  align-items: center;
}

.global-navigation_contact {
  display: grid;
  justify-items: end;
}

.global-navigation_contact {
  padding: 15px;
}

ul {
  padding: 0;
  margin: 0;
  list-style-type: none;
}

ul > li {
  display: inline-block;
  padding: 15px;
}

a {
  display: block;
  color: #ffffff;
  text-decoration: none;
  font-size: 18px;
  text-transform: uppercase;
}
</style>
