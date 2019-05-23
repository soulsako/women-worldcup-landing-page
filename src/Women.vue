<template>
  <div class="women">
    <div class="women__inner">
      <div class="women__textbox">
        <p>{{text}}</p>
        <p>{{textTwo}}</p>
      </div>
      <div class="women__countrybox">
        <div class="women__countrybox-country" v-for="(country, index) in countries" :key="index">
          <a href="/" class="women__countrybox-flag">
            <img :src="country.img" alt="" class="women__countrybox-img">
          </a>
          <p class="women__countrybox-text">{{ country.text}}</p>  
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    props: ['text', 'textTwo', 'countries']
  }
</script>

<style lang="scss" scoped>
@import './assets/scss/media.scss';
  .women {
    padding: 2.5rem;
    background-color: #f2f2f2;

    &__textbox {
      display: flex;
      justify-content: space-between;
      align-content: center;
      text-transform: uppercase;
      color: #000;
      font-weight: bold;
      p {
        font-size: 1.3rem;
        letter-spacing: 3.38px;
        line-height: 1.3rem;
      }
    }

    &__countrybox {
      display: flex;
      overflow-x: scroll;
      align-items: center;
      justify-content: space-between;
      padding: 1.5rem 0;
      text-transform: uppercase;
      width: 100vw;

      &-country {
      display: flex;
      flex-direction: column;
      align-items: center;
      min-width: 10rem;
      min-height: 10rem;
      border-radius: 20rem;
      }
      &-flag {
      width: 100%;
      height: 100%;
      margin-bottom: 1rem;
      object-fit: cover;
      }
      &-img {
      display: block;
      width: 100%;
      height: 100%;
      }
      &-text {
      font-size: 1.2rem;
      line-height: 1.8rem;
      letter-spacing: 3.12px;
      }
    }
  }
</style>