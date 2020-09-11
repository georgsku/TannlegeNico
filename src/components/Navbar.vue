<template>
  <nav >
      <img src="../assets/LogoNicoTannlege.png" class="navbar-logo" alt="">
      <div class="navbar-container">
        <div class="nav-btn" @click="navbarClick('a')">
          <img src="../assets/dentist.svg" class="nav-icon" alt="">
          <p>Om oss</p>
        </div>  
        <div class="nav-btn" @click="navbarClick('b')">
          <img src="../assets/dentist.svg" class="nav-icon" alt="">
          <p>Timebestillinger</p>
        </div>  
        <div class="nav-btn" @click="navbarClick('c')">
          <img src="../assets/dentist.svg" class="nav-icon" alt="">
          <p>Betaling</p>
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
      document.getElementById(element).scrollIntoView({behavior: "smooth", block: "center",});
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
    height: 150px;
    width: auto;
    margin: 20px 0;
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
      color: #7ac8dc;
    }

    & > img {
      height: 40px;
    }
  }
  
</style>