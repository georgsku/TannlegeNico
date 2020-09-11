<template>
  <div class="card-container shadow mx-5 p-3">
    <img :src="image" class="my-2" alt="">
  </div>
</template>

<script>
export default {
  components: {},
  props: ["image"],
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

<style lang="scss" scoped>
  .card-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 20%;
    height: 300px;

    & img {
      height: 100px;
    }
  }
</style>