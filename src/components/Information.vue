<template>
  <div class="information my-5">
    <Card 
      :image="image1"
      headline="Timebestilling"
      text="Timebestillinger gjøres på telefon, eller ved å besøke kontoret."/>
    <Card 
      :image="image2"
      headline="Akuttbehandling"
      text="Ved behov for akutt behandling vil vi alltid forsøke å hjelpe så fort vi har mulighet."/>
    <Card 
      :image="image3"
      headline="Avbestilling"
      text="Avbestilling av time må gjøres senest 24 timer før avtalt time. Om mulig setter vi pris på om det gjøres så tidlig som mulig. Ikke benyttet time vil fakturerer med 70% av timehonorar."/>
  </div>
</template>

<script>

import Card from './Card'

export default {
  components: {Card},
  props: {},
  data() {
    return {
      image1: require('../assets/undraw_booking_33fn.svg'),
      image2: require('../assets/undraw_doctors_hwty.svg'),
      image3: require('../assets/undraw_calendar_dutt.svg'),
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
    flex-direction: row;
    justify-content: center;
  }
</style>