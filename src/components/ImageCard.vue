<template>
  <div class="card-container image-card-container shadow m-4 p-3 d-none d-xl-flex">
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
    & img {
      height: 120px;
    }
  }
</style>