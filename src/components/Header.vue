<template>
  <header>
    <div class="content">
      <div class="header-image">
        <img src="https://i.imgur.com/fW6AOzf.png" alt="image">
      </div>
      <div class="header-text">
        <p>
          Om Oss
          <br>
          Tannlege Nicolay Nilssen. Ved tannlege Nilssens kontor er vi to tannleger og en tannpleier. Vi tilbyr alle former for tannbehandling. fran undersøkelse og tannrens til implantat behandling. I de tilfellene vi ikke kan løse problemet på vårt kontor samarbeider vi med lokale spesialister. Vi samarbeider også med lokale tannteknikere om fremstilling av krone og broarbeider og protesearbeider. Dette for best mulig kvalitet og for et best mulig samarbeide til pasientenes beste.
          Tannlege Nicolay Nilssen har jobbet som tannlege siden 2001. Han er også godkjent for å utføre implantatprotetisk behandling for trygdens regning. 
          Tannlege Cathrine Nylund Tingleff har jobbet som tannlege siden 2009. Tannlege tingleff har i hele sin kariere hatt en spesiell interesse for pasienten med tannlegeskrekk.
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