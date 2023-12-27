<template>
    <div class="digital d-flex flex-column align-items-center">
        <h2 class="digital-headline">What Are Digital Securities?</h2>
        <p class="digital-text">Digital securities represent traditional assets like equity or bonds.<br/>
            They carry all of the same legal rights of their paper issued counter-parts.</p>
        <div class="digital-cards-wrapper d-flex justify-content-around w-100">
            <div class="digital-cards-item d-flex flex-column justify-content-center">
                <img class="digital-cards-item-img" src="../assets/images/invest.svg" />
                <h3 class="card-headline text-center">Invest Any Amount</h3>
                <p class="card-text text-center">Start with as little as $1,<br/>buy parts of a whole share</p>
            </div>
            <div class="digital-cards-item">
                <img class="digital-cards-item-img" src="../assets/images/access.svg" />
                <h3 class="card-headline text-center">Access Private Equity</h3>
                <p class="card-text text-center">Get access to investments typically<br/>reserved for institutions</p>
            </div>
            <div class="digital-cards-item">
                <img class="digital-cards-item-img" src="../assets/images/trade.svg" />
                <h3 class="card-headline text-center">Trade 24/7</h3>
                <p class="card-text text-center">Digital assets don’t sleep,<br/>so why should you stop trading?</p>
            </div>
        </div>
        <form class="form d-flex">
            <input type="email" placeholder="E-mail*" required class="form-email form-control" />
            <button class="form-btn btn btn-success" @click="modalChange">Get Early Access</button>
        </form>
    </div>
</template>

<script>
export default {
    name: 'DigitalSecurities',
    methods: {
        modalChange() {
            this.$emit('modalChange', {isModal: true, success: true, form: false})
        },
    },
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.digital-headline{
    font-size: 2.8125rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-transform: capitalize;
    margin: 1.87rem 0;
}
.digital-text{
    margin-bottom: 2.5rem;
    text-align: center;
    font-size: 1.5625rem;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
.digital-cards-wrapper{
    margin-bottom: 3.4rem;
}
.digital-cards-item {
    max-width: 33vw;
}
.card-headline{
    margin: 2rem 0 1.08rem 0;
    font-size: 1.875rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
.card-text{
    font-size: 1.375rem;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
.digital-cards-item-img{
    max-width: 20rem;
    max-height: 20.5rem;
}
.form{
    margin-bottom: 3.06rem;
}
.form-email{
    min-width: 26.75rem;
    margin-right: 1.25rem;
}
.form-btn{
    min-width: 26.75rem;
    border: 3px solid #2ECC71 !important;
    background-color: #2ECC71;
}
.form-btn:hover{
    background-color: transparent !important;
    color: #2DC66E;
}

@media screen and (max-width: 360px){
    .digital-headline{
        text-align: center;
        font-size: 2.1875rem;
        line-height: 2rem;
        margin: 2.5rem 0 1rem 0;
    }
    .digital-text{
        text-align: center;
        font-size: 1.125rem;
    }
    .digital-cards-wrapper{
        flex-direction: column;
    }
    .card-headline{
        font-size: 1.375rem;
    }
    .card-text{
        font-size: 1.25rem;
    }
    .digital-cards-item-img{
        max-width: 14rem;
        max-height: 14rem;
        min-width: 14rem;
        min-height: 14rem;
    }
    .digital-cards-item{
        display: flex;
        flex-direction: column;
        align-items: center;
        max-width: 100%;
        margin-bottom: 2.08rem;
    }
    .form{
        flex-direction: column;
        max-width: 320px;
    }
    .form-email{
        min-width: 320px;
        margin-bottom: 18px;
    }
    .form-btn{
        min-width: 320px;
    }
}
</style>