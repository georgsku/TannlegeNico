<template>
  <div id="app">
    <Navbar />
    <Header />
    <Information />
    <Employees />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar' 
import Header from './components/Header' 
import Information from './components/Information'
import Employees from './components/Employees'
import Footer from './components/Footer' 

import 'vueperslides/dist/vueperslides.css'

export default {
  name: 'App',
  components: { Navbar, Header, Footer, Information, Employees }
}
</script>

<style lang="scss">

  body {
    color: #3c4a4d;
  }

  h1, h2, h3, h4 {
    font-family: 'Montserrat', sans-serif;
  }

  p {
    font-family: 'Baloo Tamma 2', cursive, 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }

  * {
    margin: 0;
    padding: 0;
  }

  .content {
    width: 80vw;
    max-width: 1200px;
    margin: auto;
  }
</style>

