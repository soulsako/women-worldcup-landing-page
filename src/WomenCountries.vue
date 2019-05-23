<template>
  <Women 
  :text="text"
  :textTwo="textTwo"
  :countries="countries"
  />
</template>

<script>
import Women from './Women.vue';
  export default {
    components: {Women},
    data(){
      return {
        text: 'shop by team', 
        textTwo: 'all', 
        countries: [
          { img: 'https://i8.amplience.net/i/jpl/england-2a9abea14fc86db518d8629b9cd03f5f', text: 'England' }, 
          { img: 'https://i8.amplience.net/i/jpl/usa-81114136d8eade497aa14a50016a606f', text: 'U.S.A' }, 
          { img: 'https://i8.amplience.net/i/jpl/france-dad4c62153708f9c2ca92cc772653ed6', text: 'France' }, 
          { img: 'https://i8.amplience.net/i/jpl/scotland-a2e0efa7635150140940b59fc95b2d42', text: 'scotland' }, 
          { img: 'https://i8.amplience.net/i/jpl/england-2a9abea14fc86db518d8629b9cd03f5f', text: 'England' }, 
          { img: 'https://i8.amplience.net/i/jpl/usa-81114136d8eade497aa14a50016a606f', text: 'U.S.A' }, 
          { img: 'https://i8.amplience.net/i/jpl/france-dad4c62153708f9c2ca92cc772653ed6', text: 'France' }, 
          { img: 'https://i8.amplience.net/i/jpl/scotland-a2e0efa7635150140940b59fc95b2d42', text: 'scotland' }
        ]
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>