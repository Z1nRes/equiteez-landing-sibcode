<template>
    <div class="footer d-flex flex-column">
        <div class="footer-content d-flex">
            <div class="footer-block">
              <div class="footer-logo">
                <img src="../assets/Equiteez.svg" />
              </div>
              <p class="footer-text text-white">Contacn Us</p>
              <div class="mobile-nav">
                <nav class="d-flex flex-column">
                  <a href="#" class="footer-nav-link text-decoration-none text-white">What Are Digital Securities?</a>
                  <a href="#" class="footer-nav-link text-decoration-none text-white">Products</a>
                  <a href="#" class="footer-nav-link text-decoration-none text-white">Digitize Your Business</a>
                  <a href="#" class="footer-nav-link text-decoration-none text-white">Blog</a>
                  <a href="#" class="footer-nav-link text-decoration-none text-white">Contacn Us</a>
                </nav>
              </div>
              <div class="footer-social">
                  <a href="#" class="footer-social-link"><img src="../assets/images/social/Twitter.svg" /></a>
                  <a href="#" class="footer-social-link"><img src="../assets/images/social/Facebook.svg" /></a>
                  <a href="#" class="footer-social-link"><img src="../assets/images/social/Linkedin.svg" /></a>
                  <a href="#" class="footer-social-link"><img src="../assets/images/social/Medium (1).svg" /></a>
              </div>
            </div>
            <div class="footer-block">
              <nav class="d-flex flex-column">
                <a href="#" class="footer-nav-link text-decoration-none text-white">What Are Digital Securities?</a>
                <a href="#" class="footer-nav-link text-decoration-none text-white">Products</a>
                <a href="#" class="footer-nav-link text-decoration-none text-white">Digitize Your Business</a>
                <a href="#" class="footer-nav-link text-decoration-none text-white">Blog</a>
              </nav>
            </div>
        </div>
        
        <div class="copyright">
          <hr class="copyright-line text-white">
          <p class="copyright-text text-white">©2020 Equiteez.All rights reserved.</p>
        </div>
    </div>
    
  </template>
  
  <script>
  export default {
    name: 'FooterComponent',
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.footer{
    background-color: #252525;
    height: 373px;
}
.footer-logo{
  margin-bottom: 1.19rem;
}
.footer-text{
  margin-bottom: 3.61rem;
  font-size: 1.125rem;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
}
.footer-social-link:not(:last-child){
  padding-right: 7.29px;
}
.footer-nav-link{
  font-size: 1.125rem;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
}

.footer-nav-link:not(:last-child){
  padding-bottom: 1.44rem;
}
.footer-block:first-child{
  margin: 2.06rem 0 0 18.88rem;
}
.footer-block:last-child{
  margin: 3.69rem 0 0 10.56rem;
}
.mobile-nav{
  display: none;
}
.copyright{
  font-size: 1rem;
  font-style: italic;
  font-weight: 400;
  line-height: normal;
  text-align: center;
  bottom: 0;
}
.copyright-text{
  margin: 1.56rem 0 0 0;
}
.copyright-line{
  max-width: 1322px;
  width: 82rem;
  margin: 4.94rem 0 0 18.62rem;
}
@media (min-width: 362px) and (max-width: 1366px){
  .copyright-line{
    max-width: 1145px;
    margin: 4.94rem 0 0 6.94rem;
  }
}
@media screen and (max-width: 361px){
  .copyright-line{
    max-width: 360px;
    margin: 1.25rem 0 0 0;
  }
  .footer{
    height: 537px;
  }
  .footer-content{
    flex-direction: column;
  }
  .footer-block:first-child{
    margin: 2.06rem 0 0 0;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .footer-block:last-child{
    display: none;
  }
  .footer-text{
    display: none;
  }
  .footer-logo{
    width: 10rem;
    height: 4rem;
  }
  .mobile-nav{
    text-align: center;
    margin-bottom: 1.25rem;
  }
}
</style>