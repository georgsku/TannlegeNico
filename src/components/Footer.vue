<template>
  <footer>
    <div class="content row py-4">
      <div class="col-1"></div>
      <div class="col-5 text-center">
        <h4>Adresse:</h4>
        <p style="white-space: pre-line"> Storgata 5 <br> 3520 Jevnaker</p>
      </div>
      <div class="col-5 text-center">
        <h4>Telefon:</h4>
        <p style="white-space: pre-line"> 61 31 13 79</p>
      </div>
      <div class="col-1"></div>
    </div>

  </footer>
</template>

<style lang="scss">
  footer {
    height: 180px;
    background: #3c4a4d;
    color: white;

    & > .content {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
    }
  }
</style>