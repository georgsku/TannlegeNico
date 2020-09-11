<template>
  <header>
    <div class="content">
      <div class="header-image shadow">
        <img src="https://i.imgur.com/NoQpCq5.jpg" alt="image">
      </div>
      <div class="header-text">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras in massa sapien. Quisque vitae ex vel ex eleifend sollicitudin eget sit amet ipsum. Ut in metus in lorem laoreet malesuada. Nunc ut semper nibh. Duis non faucibus lectus. Mauris id congue nisl. Cras molestie tempus neque, ac tempus ante vehicula nec. Aliquam eget luctus nulla. Etiam sit amet ante non ligula aliquet sollicitudin ac ac elit. Fusce sapien leo, volutpat nec mi id, consequat blandit ante.
        </p>
      </div>
    </div>
  </header>
</template>

<style lang="scss">
  header {
    background: #f4f8f7;
    margin-top: 40px;

    & .content {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;

      & .header-image {
        transform: translateY(-20px);

        & img {
          height: 30vh;
        }
      }

      & .header-text {
        padding: 10px 15px;
        text-align: center;
        font-size: 18px;

      }

    }
  }

</style>