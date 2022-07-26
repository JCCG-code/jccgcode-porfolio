<template>

  <Header id="topPage"/>
  <Menu/>
  <About id="about"/>
  <Portfolio id="portfolio"/>
  <Blog id="blog"/>
  <Contact id="contact"/>

</template>

<script>
import Header from './components/Header.vue'
import Menu from './components/Menu.vue'
import About from './components/About.vue'
import Portfolio from './components/Portfolio.vue'
import Blog from './components/Blog.vue'
import Contact from './components/Contact.vue'

export default {
  components: {
    Header,
    Menu,
    About,
    Portfolio,
    Blog,
    Contact
}
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  text-decoration: none;
  list-style: none;
  box-sizing: border-box;
}

body, button {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
</style>
