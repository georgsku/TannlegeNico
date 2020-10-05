<template>
  <div class="card-container shadow py-3 px-5 px-md-3 mx-2 mx-md-4 my-4">
    <img :src="image" class="my-2" alt="" v-if="image">
    <h3 class="mt-4" >{{headline}}</h3>
    <p style="white-space: pre-line">{{text}}</p>
  </div>
</template>

<script>
export default {
  components: {},
  props: ["headline", "text", "image"],
  data() {
    return {
    }
  },
  computed: {
  },
  methods: {
  },
  mounted() {
  }
}
</script>

<style lang="scss">
  .card-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 350px;
    border-radius: 30px;
    margin: 10px 0;

    & h3 {
      color: #3c4a4d;
      font-size: 23px;
    }

    & p {
      text-align: center;
    }

    & img {
      height: 50px;
    }
  }

  .card-container:hover {
    transform: scale(1.02) translateY(-3px);
    box-shadow: 0 0.5rem 1.2rem rgba(0, 0, 0, .15)!important;
  }

  .card-container {
    flex: 1 0 26%;
  }

  @media screen and (max-width: 1200px) {
    .card-container {
      flex: 1 0 34%;
    }
  }

  @media screen and (max-width: 768px) {
    .card-container {
      flex: 1 0 51%;
    }
  }
  

</style>