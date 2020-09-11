<template>
  <nav >
      <img src="../assets/tooth2.svg" class="navbar-logo mt-4" alt="">
      <h1 class="font-weight-bolder m-0" style="color: #30c9e8">Tannlege</h1>
      <h4 style="color: #30c9e8">&mdash; Nicolay Nilssen &mdash;</h4>
      <div class="navbar-container mt-1">
        <div class="nav-btn" @click="navbarClick('header')">
          <img src="../assets/dentist.svg" alt="">
          <p>Om oss</p>
        </div>  
        <div class="nav-btn" @click="navbarClick('.first-info')">
          <img src="../assets/dentist.svg" alt="">
          <p>Timebestillinger</p>
        </div>  
        <div class="nav-btn" @click="navbarClick('.second-info')">
          <img src="../assets/dentist.svg" alt="">
          <p>Åpningstider</p>
        </div>  
        <div class="nav-btn" @click="navbarClick('.employee')">
          <img src="../assets/dentist.svg" alt="">
          <p>Ansatte</p>
        </div> 
      </div>  
  </nav>
</template>

<script>
export default {
  components: {},
  props: {},
  data() {
    return {
    }
  },
  computed: {
  },
  methods: {
    navbarClick(element) {
      document.querySelector(element).scrollIntoView({behavior: "smooth", block: "center",});
    }
  },
  mounted() {
  }
}
</script>

<style lang="scss">

  nav {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .navbar-logo {
    height: 90px;
    width: auto;
  }

  .navbar-container {
    display: flex;
    flex-direction: row;
    justify-content: center;
  }

  .nav-btn {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 0 30px;
    cursor: pointer;

    & > p {
      font-size: 17px;
      margin: 5px 0;
      color: #30c9e8;
      font-weight: 600;
    }

    & > img {
      height: 40px;
    }
  }
  
</style>