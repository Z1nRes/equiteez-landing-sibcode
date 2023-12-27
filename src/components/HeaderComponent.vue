<template>
  <div class="header d-flex justify-content-between align-items-center ">
    <div class="header-logo">
      <img src="../assets/Equiteez.svg" />
    </div>
    <div class="burger-btn" @click="changeBurger">
      <img src="../assets/images/burger_menu.svg" />
    </div>
    <div class="header-nav">
      <nav class="d-flex">
        <a href="#" class="header-nav-link text-decoration-none text-black">What Are Digital Securities?</a>
        <a href="#" class="header-nav-link text-decoration-none text-black">Products</a>
        <a href="#" class="header-nav-link text-decoration-none text-black">Digitize Your Business</a>
        <a href="#" class="header-nav-link text-decoration-none text-black">Blog</a>
        <a href="#" class="header-nav-link text-decoration-none text-black">Contact Us</a>
      </nav>
    </div>
    <div class="header-social">
      <a href="#" class="header-social-link"><img src="../assets/images/social/Twitter.svg" /></a>
      <a href="#" class="header-social-link"><img src="../assets/images/social/Facebook.svg" /></a>
      <a href="#" class="header-social-link"><img src="../assets/images/social/Linkedin.svg" /></a>
      <a href="#" class="header-social-link"><img src="../assets/images/social/Medium.svg" /></a>
    </div>
  </div>

  <div :class="[showBurger ? 'd-flex' : 'hidden']" class="burger-menu flex-column">
    <nav class="d-flex flex-column">
      <a href="#" class="header-nav-link text-decoration-none text-black">What Are Digital Securities?</a>
      <a href="#" class="header-nav-link text-decoration-none text-black">Products</a>
      <a href="#" class="header-nav-link text-decoration-none text-black">Digitize Your Business</a>
      <a href="#" class="header-nav-link text-decoration-none text-black">Blog</a>
      <a href="#" class="header-nav-link text-decoration-none text-black">Contact Us</a>
    </nav>
    <div class="header-social-burger">
      <a href="#" class="header-social-link"><img src="../assets/images/social/Twitter (Traced).svg" /></a>
      <a href="#" class="header-social-link"><img src="../assets/images/social/Facebook (Traced).svg" /></a>
      <a href="#" class="header-social-link"><img src="../assets/images/social/Linkedin (Traced).svg" /></a>
      <a href="#" class="header-social-link"><img src="../assets/images/social/Medium (3).svg" /></a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent',
  data() {
    return{
      showBurger: false,
    }
  },
  methods: {
    changeBurger() {
      if (this.showBurger === false) {
        this.showBurger = true
      } else {
        this.showBurger = false
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header{
  height: 105px;
  box-shadow: 0px 1px 10px 0px rgba(0, 0, 0, 0.25);
  padding: 0 18.88rem;
}
.header-logo{
  cursor: pointer;
}
.burger-btn{
    display: none;
}
.header-nav-link{
  font-weight: 600;
  size: 18px;
}
.header-nav-link:not(:last-child){
  padding-right: 22px;
}
.header-social-link:not(:last-child){
  padding-right: 7.29px;
}
.hidden{
  display: none;
}
@media (min-width: 361px) and (max-width: 1366px){
  .header{
    padding: 0 6.94rem;
  }
}
@media screen and (max-width: 360px){
  .header-logo{
    margin-right: 3rem;
  }
  .header-nav{
    display: none;
  }
  .header-social{
    display: none;
  }
  .header{
    padding: 0 6rem;
  }
  .burger-btn{
    display: block;
    width: 25px;
    height: 25px;
  }
  .burger-menu{
    position: absolute;
    z-index: 99;
    padding-left: 1.25rem;
    padding-top: 1.63rem;
    width: 100%;
    height: 17rem;
    background-color: #2ECC71;
  }
  .header-social-burger{
    margin-top: 2.63rem;
  }
  .header-nav-link:not(:last-child){
    margin-bottom: 0.31rem;
  }
}
</style>
