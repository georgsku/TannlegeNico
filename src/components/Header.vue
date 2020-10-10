<template>
  <header>
    <div class="content">
      <div class="header-image shadow mr-md-4 mr-0 rounded-image"></div>
      <div class="header-text py-5 pl-4">
        <h1>Velkommen til tannlege Nicolay Nilssen</h1>
        <p style="font-size: 22px">Ved Nilssens kontor er vi to tannleger og en tannpleier. Vi tilbyr alle former for tannbehandling, 
          fra undersøkelse og tannrens til implantatbehandling. Vi samarbeider med lokale spesialister og tannteknikere; 
          for å oppnå best mulig resultat for pasienten.</p>
      </div>
    </div>
  </header>
</template>

<style lang="scss">

  header {
    background: #88d8e5;
    margin-top: 40px;
    color: #f4f8f7;
    min-height: 700px;
    padding: 50px 0;
    display: flex;
    border-top: solid 10px #f4f8f7;
    border-bottom: solid 10px #f4f8f7;

    & .content {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
      min-height: 350px;

      & .header-image {
        width: 60%;
        height: inherit;
        min-height: 300px;
        transform: translateY(-20px);
        background-image: url('https://i.imgur.com/NoQpCq5.jpg');
        background-position: center;
        background-size: cover;
        border-radius: 30px;
        border: solid 6px white;

      }

      .header-image:hover {
        transform: translateY(-23px);
        box-shadow: 0 0.5rem 1.2rem rgba(0, 0, 0, .15)!important;
      }

      & .header-text {
        padding: 10px 15px;
        text-align: center;
        font-size: 18px;
        width: 50%;
        display: flex;
        flex-direction: column;
        align-items: center;
      }

    }
  }

  @media only screen and (max-width: 768px) {

    header {
      height: auto;
      padding: 0;
    }
        
    header .content {
      flex-direction: column;
      align-items: center;
      width: 90%;

      & .header-text{
        width: 90%;
      }
      & .header-image{
        width: 70%;
      }
    }

    


  }

</style>