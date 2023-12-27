<template>
  <HeaderComponent />
  <div class="container">
    <PrivateEquity @modalChange="modalChange" />
    <DigitalSecurities @modalChange="modalChange" />
  </div>
  <LozungComponent />
  <div class="container">
    <ProductsComponent />
  </div>
  <div class="triangle-up"></div>
  <div class="bg-gray">
    <div class="container">
      <DigitizeYourBusiness />
    </div>
  </div>
  <div class="triangle-down"></div>
  <div class="container">
      <BlogComponent @modalChange="modalChange" />
  </div>
  <div class="bg-gray">
    <div class="container">
      <ContactUs @modalChange="modalChange" />
    </div>
  </div>
  <FooterComponent />
  <div
    @click="modalChange({isModal: false, success: false, form: false})"
    :class="[isModal ? 'd-flex' : 'hidden']"
    class="modal-window justify-content-center align-items-center">
    <div :class="[success ? 'd-block' : 'hidden']">
      <SuccessModal @modalChange="modalChange" />
    </div>
    <div class="modal-signup" :class="[form ? 'd-block' : 'hidden']">
      <h3 class="modal-signup-headline">Singnup For Free</h3>
      <ContactForm @modalChange="modalChange" />
    </div>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import PrivateEquity from './components/PrivateEquity.vue'
import DigitalSecurities from './components/DigitalSecurities.vue'
import LozungComponent from './components/LozungComponent.vue'
import ProductsComponent from './components/ProductsComponent.vue'
import DigitizeYourBusiness from './components/DigitizeYourBusiness.vue'
import BlogComponent from './components/BlogComponent.vue'
import ContactUs from './components/ContactUs.vue'
import ContactForm from './components/ContactForm.vue'
import FooterComponent from './components/FooterComponent.vue'
import SuccessModal from './components/SuccessModal.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    PrivateEquity,
    DigitalSecurities,
    LozungComponent,
    ProductsComponent,
    DigitizeYourBusiness,
    BlogComponent,
    ContactUs,
    ContactForm,
    FooterComponent,
    SuccessModal,
  },
  data() {
    return{
      isModal: false,
      success: false,
      form: false
    }
  },
  methods: {
    modalChange(data) {
        this.isModal = data.isModal
        this.success = data.success
        this.form = data.form
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Open Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  -ms-overflow-style: none;  /* IE и Edge */
  scrollbar-width: none;  /* Firefox */
}
body::-webkit-scrollbar {
  display: none;
}
.triangle-up{
  border-bottom: 68.5px solid rgba(196, 196, 196, .25);
  border-right: 1920px solid transparent;
}
.triangle-down{
  border-bottom: 68.5px solid rgba(196, 196, 196, .25);
  border-right: 1920px solid transparent;
  transform: scale(1, -1);
}
.bg-gray{
  background-color: rgba(196, 196, 196, .25);
}
.modal-window{
  position: fixed;
  top: 0;
  left: 0;
  z-index: 99;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, .3);
}
.hidden{
  display: none;
}
.modal-signup{
  border-radius: 0.625rem;
  background-color: #fff;
  padding: 0 1.3rem 1.06rem 1.3rem;
}
.modal-signup-headline{
  text-align: center;
  font-size: 1.25rem;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
  padding: 1.62rem 0 3.63rem 0;
}

@media (min-width: 361px) and (max-width: 1366px){
  .triangle-up{
    border-right: 1366px solid transparent;
  }
  .triangle-down{
    border-right: 1366px solid transparent;
  }
}
@media screen and (max-width: 360px){
  .triangle-up{
  border-right: 360px solid transparent;
  }
  .triangle-down{
    border-right: 360px solid transparent;
  }
}
</style>
