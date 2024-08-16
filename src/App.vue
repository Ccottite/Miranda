<template>
  <div id="app">
    <Navbar />
    <Home />
    <Partners />
    <Products />
    <MNew />
    <Contact />
    <Footer />

  </div>
</template>

<script>
import Navbar from './components/MainNavbar.vue';
import Home from './components/MirandaHome.vue';
import Partners from './components/MirandaPartners';
import Products from './components/MirandaProducts';
import MNew from './components/MirandaNew';
import Contact from './components/MirandaContact';
import Footer from './components/MirandaFooter.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    Partners,
    Products,
    MNew,
    Contact,
    Footer
  }
}
</script>

<style></style>
