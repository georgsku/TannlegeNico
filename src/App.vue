<template>
  <div id="app">
    <Navbar />
    <Header />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar' 
import Header from './components/Header' 
import Footer from './components/Footer' 


export default {
  name: 'App',
  components: { Navbar, Header, Footer }
}
</script>

<style lang="scss">

  p, h1, h2, h3, h4 {
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }

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
