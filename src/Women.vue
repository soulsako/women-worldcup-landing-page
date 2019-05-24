<template>
  <div class="women" :style="{backgroundColor: backgroundColor}">
    <div class="women__inner">
      <div class="women__textbox">
        <p>{{text}}</p>
        <p>{{textTwo}}</p>
      </div>
      <div class="women__countrybox">
        <div class="women__countrybox-country" v-for="(country, index) in data" :key="index">
          <a href="/" class="women__countrybox-flag">
            <picture class="women__countrybox-img">
              <source :srcset="country.img" media="(max-width: 37.5em)">
              <img :src="country.img2" alt="Country Logos">
            </picture>
          </a>
          <p class="women__countrybox-text">{{ country.text}}</p>  
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    props: ['text', 'textTwo', 'data', 'country'], 
    computed: {
      backgroundColor(){
        return this.country ? '#f2f2f2' : '#fff'
      }
    }
  }
</script>

<style lang="scss" scoped>
@import './assets/scss/media.scss';
  .women {
    padding: 2.5rem;
    @include desktop {
          padding: 5rem 20rem;
        }
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
        @include desktop {
          font-size: 2.8rem;
          letter-spacing: 7.28px;
          line-height: 3rem;
        }
        &:last-child{
          text-decoration: underline;
        }
      }
    }

    &__countrybox {
      display: flex;
      overflow-x: scroll;
      align-items: center;
      padding: 1.5rem 0;
      text-transform: uppercase;
      @include desktop {
        padding: 3rem 0;
      }
      &-country {
      display: flex;
      flex-direction: column;
      align-items: center;
      &:not(:last-child){
        margin-right: 5rem;
        }
      }
      &-flag {
      margin-bottom: .5rem;
      object-fit: contain;
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
      @include desktop {
          font-size: 2rem;
          line-height: 3.2rem;
          letter-spacing: 5.2px;
        }
      }
    }
  }
</style>