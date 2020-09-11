<template>
  <div class="card-container shadow mx-5 p-3">
    <img :src="image" class="my-2" alt="">
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
    width: 20%;
    height: 350px;
    border-radius: 30px;

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
    transform: scale(1.03) translateY(-6px);
    box-shadow: 0 0.5rem 2rem rgba(0, 0, 0, .15)!important;
  }

</style>