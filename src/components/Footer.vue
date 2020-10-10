<template>
  <footer>
    <div class="content row">
      <div class="offset-md-1 col-md-5 col-12 text-center pt-4 align-center">
        <a href="https://goo.gl/maps/UdvmzoQA1Y4SGwzx9" target="__blank" title="Åpne i Google Maps" class="shadow"  id="footer-map">
          <img src="../assets/map.png" alt="map">
        </a>
        <!-- <a href="https://goo.gl/maps/UdvmzoQA1Y4SGwzx9" target="__blank" title="Åpne i Google Maps">
          <img src="../assets/undraw_Map_dark_k9pw.svg" alt="map" style="height: 50px;">
        </a> -->
      </div>
      <div class="col-md-5 col-12 text-center pt-4 d-flex flex-column justify-content-center">
        <h4>Adresse:</h4>
        <p class="mb-0" style="white-space: pre-line"> Storgata 5 <br> 3520 Jevnaker</p>
        <br>
        <h4>Telefon:</h4>
        <p style="white-space: pre-line"> 
          <a href="tel:61311379">61 31 13 79</a> <br> 
          <span class="text-muted">Vi har telefontid i hele åpningstiden. Ved stor pågang har vi tidvis problemer med å besvare alle anrop. Vennligst ring tilbake litt senere!</span>
        </p>
      </div>
    </div>

  </footer>
</template>

<style lang="scss">
  footer {
    background: #3c4a4d;
    color: white;

    a, a:visited, a:hover, a:active {
      color: white;
      text-decoration: underline;
    }
  }

  #footer-map {
    border: 6px solid white;
    display: block;
    border-radius: 30px;
    width: 350px;
    max-width: 100%;
    margin: 20px auto 40px;
    overflow: hidden;

    & img {
      max-width: 100%;
      max-height: 350px;
      
    }

    &:hover {
        transform: translateY(-4px);
        box-shadow: 0 0.5rem 1.2rem rgba(0, 0, 0, .15)!important;
    }
  }

  @media only screen and (max-width: 550px) {

    footer .content {
      flex-direction: column;
      align-items: center;
    }

  }



</style>