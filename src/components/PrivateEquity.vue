<template>
    <div class="equity d-flex align-items-center">
        <div class="equity-content d-flex flex-column">
            <h1 class="equity-content-headline">Private Equity Made Easy</h1>
            <div class="mobile-img"><img src="../assets/images/phone.svg"/></div>
            <p class="equity-content-text">Equiteez is on a mission to make private equity easily accesible to all in vestors</p>
            <button class="equity-content-btn btn btn-dark" @click="modalChange" >Signnup For Free</button>
        </div>
        <div class="equity-img">
            <img src="../assets/images/phone.svg"/>
        </div>
        <div class="equity-bg d-flex"></div>
    </div>
</template>

<script>
export default {
name: 'PrivateEquity',
methods: {
    modalChange() {
        this.$emit("modalChange", {isModal: true, success: false, form: true})
    }
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
* {
    color: #fff;
}

.equity{
    height: 769px;
}
.equity-content{
    width: 652px;
}
.equity-content-headline{
    font-size: 52px;
    font-weight: 700;
    white-space: nowrap;
    padding-bottom: 30px;
}
.equity-content-text{ 
    font-size: 32px;
    line-height: 44px;
    padding-bottom: 48px;
}
.equity-content-btn{
    max-width: 255px;
    padding: 14px 0 15px 0;
    font-size: 20px;
    font-weight: 500;
    line-height: 27px;
}
.btn-dark{
    border: 3px solid #252525 !important;
}
.btn-dark:hover{
    background-color: transparent !important;
    color: #000;
}
.equity-img{
    width: 35vw;
}
.mobile-img{
    display: none;
}
.equity-bg{
    width: 100%;
    height: 769px;
    position: absolute;
    z-index: -1;
    left: 0;
    background-color: #2ECC71;
}
@media (min-width: 361px) and (max-width: 1366px){
    .equity-img{
        overflow: hidden;
    }
    .equity-img > img{
        position: relative;
        left: -185px;
    }
}
@media screen and (max-width: 360px){
    .equity{
        flex-direction: column;
        height: 706px;
    }
    .equity-content{
        width: 300px;
    }
    .equity-content-headline{
        font-size: 2.1875rem;
        font-style: normal;
        font-weight: 700;
        line-height: 2.5rem;
        white-space: wrap;
        text-align: center;
        padding-top: 7px;
        padding-bottom: 0;
    }
    .equity-content-text{ 
        text-align: center;
        font-size: 1.375rem;
        font-style: normal;
        font-weight: 600;
        line-height: 1.5625rem;
        padding-bottom: 28px;
    }
    .equity-img{
        display: none;
    }
    .mobile-img{
        display: block;
        width: 320px;
        height: 400px;
        overflow: hidden;
    }
    .mobile-img > img{
        width: 470px;
        height: auto;
        position: relative;
        left: -80px;
        top: -40px;
    }
    .equity-bg{
        height: 706px;
    }
    .equity-content-btn{
        max-width: 300px;
        width: 100%
    }
}
</style>