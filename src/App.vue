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

</style>
