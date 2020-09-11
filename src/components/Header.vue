<template>
  <header>
    <div class="content">
      <div class="header-image shadow mr-4 rounded-image"></div>
      <div class="header-text py-5 pl-4">
        <h2>Om oss</h2>
          <p>Ved tannlege Nilssens kontor er vi to tannleger og en tannpleier. Vi tilbyr alle former for tannbehandling. fran undersøkelse og tannrens til implantat behandling. I de tilfellene vi ikke kan løse problemet på vårt kontor samarbeider vi med lokale spesialister. Vi samarbeider også med lokale tannteknikere om fremstilling av krone og broarbeider og protesearbeider. Dette for best mulig kvalitet og for et best mulig samarbeide til pasientenes beste.</p>
      </div>
    </div>
  </header>
</template>

<style lang="scss">
  header {
    background: #30c9e8;
    margin-top: 40px;
    color: #f4f8f7;

    & .content {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;

      & .header-image {
        width: 50%;
        height: inherit;
        transform: translateY(-20px);
        background-image: url('https://i.imgur.com/NoQpCq5.jpg');
        background-position: center;
        background-size: cover;
        border-radius: 30px;

      }

      & .header-text {
        padding: 10px 15px;
        text-align: center;
        font-size: 18px;
        width: 50%;

      }

    }
  }

</style>