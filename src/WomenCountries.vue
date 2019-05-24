<template>
  <Women 
  :text="text"
  :textTwo="textTwo"
  :data="countries"
  :country="country"
  />
</template>

<script>
import Women from './Women.vue';
const smallEng = 'https://i8.amplience.net/i/jpl/england-2a9abea14fc86db518d8629b9cd03f5f';
const smallUSA = 'https://i8.amplience.net/i/jpl/usa-81114136d8eade497aa14a50016a606f';
const smallFrance = 'https://i8.amplience.net/i/jpl/france-dad4c62153708f9c2ca92cc772653ed6';
const smallScotland = 'https://i8.amplience.net/i/jpl/scotland-a2e0efa7635150140940b59fc95b2d42';
const BigEng = 'https://i8.amplience.net/i/jpl/england-46abbd8ef29afbdb05760befa96d94a1';
const BigUSA = 'https://i8.amplience.net/i/jpl/usa-64e14ded895c917283385eb7b43eb949';
const BigFrance = 'https://i8.amplience.net/i/jpl/france-f047852540c9182fb9dd2aa4e00d09a4';
const BigScotland = 'https://i8.amplience.net/i/jpl/scotland-c540d1f060b3af189c9d3be42454a2d2';
  export default {
    components: { Women },
    data(){
      return {
        text: 'shop by team', 
        textTwo: 'all',
        country: true, 
        countries: [
          { img: smallEng, text: 'England',  img2: BigEng}, 
          { img: smallUSA, text: 'U.S.A', img2: BigUSA }, 
          { img: smallFrance, text: 'France', img2: BigFrance }, 
          { img: smallScotland, text: 'scotland', img2: BigScotland },
          { img: smallEng, text: 'England',  img2: BigEng}, 
          { img: smallUSA, text: 'U.S.A', img2: BigUSA }, 
          { img: smallFrance, text: 'France', img2: BigFrance }, 
          { img: smallScotland, text: 'scotland', img2: BigScotland } 
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>