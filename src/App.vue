<template>
  <div id="app">
    <Navbar />
    <Header />
    <Footer />
    <Employees />
  </div>
</template>

<script>
import Navbar from './components/Navbar' 
import Header from './components/Header' 
import Employees from './components/Employees'
import Footer from './components/Footer' 

import 'vueperslides/dist/vueperslides.css'

export default {
  name: 'App',
  components: { Navbar, Header, Footer, Employees }
}
</script>

<style lang="scss">
  * {
    margin: 0;
    padding: 0;
  }

  .content {
    width: 90vw;
    max-width: 1200px;
    margin: auto;
  }
</style>
