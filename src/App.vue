<template>
  <div id="app">
    <Navbar />
    <Home />
    <Partners />
    <Products />
    <MNew/>
  </div>
</template>

<script>
import Navbar from './components/MainNavbar.vue';
import Home from './components/MirandaHome.vue';
import Partners from './components/MirandaPartners';
import Products from './components/MirandaProducts';
import MNew from './components/MirandaNew';

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    Partners,
    Products,
    MNew
  }
}
</script>

<style>
/* Estilos globales */
</style>
