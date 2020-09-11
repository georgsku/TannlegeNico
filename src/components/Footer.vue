<template>
  <footer>
    <div class="content row">
      <div class="col-1"></div>
      <div class="col-5 text-center pt-4">
        <h4>Adresse:</h4>
        <p class="mb-0" style="white-space: pre-line"> Storgata 5 <br> 3520 Jevnaker</p>
        <a href="https://goo.gl/maps/a3LvtpqNv5ywWJtZ7" target="__blank" title="Åpne i Google Maps">
          <img src="../assets/undraw_Map_dark_k9pw.svg" alt="map" style="height: 50px;">
        </a>
      </div>
      <div class="col-5 text-center pt-4">
        <h4>Telefon:</h4>
        <p style="white-space: pre-line"> 
          <a href="tel:61311379">61 31 13 79</a> <br> 
          <span class="text-muted">Vi har telefontid i hele åpningstiden. Ved stor pågang har vi tidvis problemer med å besvare alle anrop. Vennligst ring tilbake litt senere!</span>
        </p>
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

    a, a:visited, a:hover, a:active {
      color: white;
      text-decoration: underline;
    }
  }


</style>