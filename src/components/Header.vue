<template>
  <header>
    <div class="content">
      <div class="header-image">
        <img src="https://i.imgur.com/fW6AOzf.png" alt="image">
      </div>
      <div class="header-text">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras in massa sapien. Quisque vitae ex vel ex eleifend sollicitudin eget sit amet ipsum. Ut in metus in lorem laoreet malesuada. Nunc ut semper nibh. Duis non faucibus lectus. Mauris id congue nisl. Cras molestie tempus neque, ac tempus ante vehicula nec. Aliquam eget luctus nulla. Etiam sit amet ante non ligula aliquet sollicitudin ac ac elit. Fusce sapien leo, volutpat nec mi id, consequat blandit ante.
          Curabitur egestas vestibulum enim, nec tempus odio interdum sed. Proin sit amet est nec mauris fermentum convallis a sed elit. Phasellus gravida leo sed commodo malesuada. Quisque eget nisl nisl. Integer nec ligula varius, ullamcorper odio tristique, tempor velit. Etiam vitae diam blandit, vestibulum ante tempor, sagittis lorem. Nulla fringilla est ut ante vulputate dapibus. Curabitur ut porta erat. Nam ac nisl egestas, finibus justo ut, pretium justo. Fusce porttitor nibh et tellus mattis, sit amet iaculis enim eleifend. Duis faucibus rhoncus eros eu volutpat. Phasellus eu leo vitae massa sagittis tempor non et est. Vivamus bibendum purus erat, at commodo lacus bibendum non.
        </p>
      </div>
    </div>
  </header>
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
  },
  mounted() {
  }
}
</script>

<style lang="scss">
  header {
    background: rgb(104, 127, 172);
    margin-top: 40px;

    & .content {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;

      & .header-image {
        transform: scaleY(1.2);

        & img {
          height: 30vw;
        }
      }

      & .header-text {
        padding: 10px 15px;
        text-align: center;
        font-size: 18px;
          color: white;

      }

    }
  }

</style>