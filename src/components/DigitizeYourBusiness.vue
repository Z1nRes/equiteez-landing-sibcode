<template>
    <div class="business">
        <h2 class="business-headlline">Digitize Your Business</h2>
        <div class="cards-wrapper d-flex">

            <div class="row">
                <div class="col">
                    <div class="card d-flex justify-content-center align-items-center">
                        <img class="card-img" src="../assets/images/business/raise_capital.svg" />
                        <h3 class="card-headline">Raise Capital</h3>
                        <p class="card-text">Expand your investor base<br/>globally through the Equitees<br/>launchpad</p>
                    </div>
                    <div class="card d-flex justify-content-center align-items-center">
                        <img class="card-img" src="../assets/images/business/lower_fees.svg" />
                        <h3 class="card-headline">Lower Fees</h3>
                        <p class="card-text">Removing unnecesary<br/>middlemen helps keep more<br/>money in your business</p>
                    </div>
                </div>
                <div class="col">
                    <div class="card d-flex justify-content-center align-items-center">
                        <img class="card-img" src="../assets/images/business/automated_compliance.svg" />
                        <h3 class="card-headline">Automated Compliance</h3>
                        <p class="card-text">Regulation aware shares<br/>means less time on the phone<br/>with your lawyers</p>
                    </div>
                    <div class="card d-flex justify-content-center align-items-center">
                        <img class="card-img" src="../assets/images/business/brand_engagement.svg" />
                        <h3 class="card-headline">Brand Engagement</h3>
                        <p class="card-text">Increase your customer<br/>engagement by rewardind<br/>your most loyal patrons</p>
                    </div>
                </div>
                <div class="col">
                    <div class="card d-flex justify-content-center align-items-center">
                        <img class="card-img" src="../assets/images/business/digital_transfer_agent.svg" />
                        <h3 class="card-headline">Digital Transfer Agent</h3>
                        <p class="card-text">Everything from shareholder ,<br/>managment, voting, even<br/>dividend distribution</p>
                    </div>
                    <div class="card d-flex justify-content-center align-items-center">
                        <img class="card-img" src="../assets/images/business/liquidity.svg" />
                        <h3 class="card-headline">24/7 Liquidity</h3>
                        <p class="card-text">Sacondary trading is hard,<br/>we make it easy though the<br/>Equiteez Marketplace</p>
                    </div>
                </div>
            </div>

        </div>
    </div>
</template>

<script>
    export default {
        name: 'DigitizeYourBusiness',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.business-headlline{
    text-align: center;
    font-size: 2.8125rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    padding: 0.69rem 0 2.44rem 0;
}
.cards-wrapper{
    padding-bottom: 2.63rem;
}
.card{
    width: 25.75rem;
    height: 19.625rem;
    border-radius: 0.625rem;
    border: 1px solid #2ECC71;
}
.card:not(:last-child){
    margin-bottom: 1.25rem;
}
.card-img {
    max-width: 3.84469rem;
    max-height: 3.8405rem;
    margin-bottom: 1.37rem;
}
.card-headline{
    font-size: 1.5625rem;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    margin-bottom: 1.37rem;
}
.card-text{
    text-align: center;
    font-size: 1.125rem;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
@media (min-width: 361px) and (max-width: 1366px){
    .card{
        width: 20.75rem;
        height: 16.625rem;
    }
}
@media screen and (max-width: 361px){
    .card{
        width: 20rem;
        height: 14.25rem;
        margin-bottom: 1.25rem;
    }
    .cards-wrapper{
        padding-bottom: 1.38rem;
    }
    .business-headline{
        font-size: 2.1875rem;
        line-height: 2.84375rem;
    }
}
</style>