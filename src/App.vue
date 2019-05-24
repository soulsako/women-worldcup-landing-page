<template>
  <div>
    <WomenCountries />
    <WomenAccessories />
    <WomenPlayers />
  </div>
</template>

<script>
import WomenCountries from './WomenCountries.vue';
import WomenAccessories from './WomenAccessories.vue';
import WomenPlayers from './WomenPlayers.vue';
export default {
  name: 'app', 
  components: { WomenCountries, WomenAccessories }
  
}
</script>

<style lang="scss" scoped>
@import './assets/scss/media.scss';
  
  
</style>
