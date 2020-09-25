<template>
  <header>
    <div class="content">
      <div class="header-image shadow mr-md-4 mr-0 rounded-image"></div>
      <div class="header-text py-5 pl-4">
        <h2>Velkommen til tannlege Nicolay Nilssen. Bestill en time hos oss via telefon. Du finner oss i Storgata 5, Jevnaker. </h2>
      </div>
    </div>
  </header>
</template>

<style lang="scss">

  header {
    background: #88d8e5;
    margin-top: 40px;
    color: #f4f8f7;

    & .content {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
      min-height: 350px;

      & .header-image {
        width: 50%;
        height: inherit;
        min-height: 300px;
        transform: translateY(-20px);
        background-image: url('https://i.imgur.com/NoQpCq5.jpg');
        background-position: center;
        background-size: cover;
        border-radius: 30px;

      }

      .header-image:hover {
        transform: scale(1.02) translateY(-23px);
        box-shadow: 0 0.5rem 1.2rem rgba(0, 0, 0, .15)!important;
      }

      & .header-text {
        padding: 10px 15px;
        text-align: center;
        font-size: 18px;
        width: 50%;
        display: flex;
        align-items: center;
      }

    }
  }

  @media only screen and (max-width: 768px) {
        
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