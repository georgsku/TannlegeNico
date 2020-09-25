<template>
  <div class="information content" style="margin: 50px auto">
    <Card 
      :image="image1"
      headline="Timebestilling"
      text="Timebestillinger gjøres på telefon, eller ved å besøke kontoret."/>
    <Card 
      :image="image2"
      headline="Akuttbehandling"
      text="Ved behov for akutt behandling vil vi alltid forsøke å hjelpe så fort vi har mulighet."/>
    <ImageCard 
      :image="image2"/>
    <ImageCard 
      :image="image1"/>
    <Card 
      :image="image3"
      headline="Avbestilling"
      text="Avbestilling av time må gjøres senest 24 timer før avtalt time. Om mulig setter vi pris på om det gjøres så tidlig som mulig. Ikke benyttet time vil fakturerer med 70% av timehonorar."/>
    <Card 
      :image="image4"
      headline="Åpningstider"
      text="Mandag: 08.30-15.30
        Tirsdag: 08.30-15.30
        Onsdag: 08.30-15.30
        Torsdag: 08.30-15.30
        Fredag: 08.30-15.00"/>
  </div>
</template>

<script>

import Card from './Card'
import ImageCard from './ImageCard'

export default {
  components: {Card, ImageCard},
  props: {},
  data() {
    return {
      image1: require('../assets/undraw_booking_33fn.svg'),
      image2: require('../assets/undraw_doctors_hwty.svg'),
      image3: require('../assets/undraw_calendar_dutt.svg'),
      image4: require('../assets/undraw_time_management_30iu.svg'),
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
  .information {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }
</style>