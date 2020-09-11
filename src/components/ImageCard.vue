<template>
  <div class="card-container image-card-container shadow mx-5 p-3">
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
  .image-card-container {
    justify-content: center;

    & img {
      height: 120px;
    }
  }
</style>