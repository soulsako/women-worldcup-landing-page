<template>
  <Women 
  :text="text"
  :textTwo="textTwo"
  :data="accessories"
  :players="players"
  />
</template>

<script>
import Women from './Women.vue';
const smallFootball = 'https://i8.amplience.net/i/jpl/image-be89bc8a7446a58bb2ba615ee7c64f9f';
const smallPads = 'https://i8.amplience.net/i/jpl/image-41776a35ce6e9a5d3dd2b2cdb9bed24f';
const smallGloves = 'https://i8.amplience.net/i/jpl/france-dad4c62153708f9c2ca92cc772653ed6';
const smallBag = 'https://i8.amplience.net/i/jpl/france-dad4c62153708f9c2ca92cc772653ed6';
const BigFootball = 'https://i8.amplience.net/i/jpl/image-81c4b75019586469a1bcf57b3ea7a3aa';
const BigPads = 'https://i8.amplience.net/i/jpl/image-d3c4cfbf8bf8ff5932d8b4a52868a463';
const BigGloves = 'https://i8.amplience.net/i/jpl/image-3c793a53abd86aad0b16218939f59bcc';
const BigBag = 'https://i8.amplience.net/i/jpl/image-7d0331153b8797e09a13c10586e44a6c';
  export default {
    components: { Women },
    data(){
      return {
        text: 'shop by player',
        textTwo: 'all',
        players: true,  
        accessories: [
          { img: smallFootball, text: 'footballs',  img2: BigFootball}, 
          { img: smallPads, text: 'shin pads', img2: BigPads }, 
          { img: smallGloves, text: 'gloves', img2: BigGloves }, 
          { img: smallBag, text: 'bags', img2: BigBag },
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>