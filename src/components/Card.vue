<template>
  <div class="card-container shadow mx-4 p-3">
    <img :src="image" class="my-2" alt="">
    <h3 class="mt-4" >{{headline}}</h3>
    <p>{{text}}</p>
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
    height: 300px;

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
</style>