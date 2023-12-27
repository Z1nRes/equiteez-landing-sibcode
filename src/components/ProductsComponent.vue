<template>
    <div class="products d-flex flex-column align-items-center">
        <h2 class="products-headline">Products</h2>
        <div class="products-content-wrapper d-flex align-items-center">
            <div class="products-content">
                <div class="products-content-block">
                    <h3 class="products-content-block-headline text-dark">Launchpad</h3>
                    <p class="products-content-block-text">Help launch startups<br/>& fund private bussinesses</p>
                </div>
                <div class="products-content-block">
                    <h3 class="products-content-block-headline">Marketplace</h3>
                    <p class="products-content-block-text">Browse through stocks on sale<br/>from private investors</p>
                </div>
            </div>

            <img src="../assets/images/phone_front.svg" />
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ProductsComponent',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.products-headline{
    margin-top: 2.69rem;
    font-size: 2.8125rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
.products-content-wrapper{
    margin-bottom: 1.66rem;
}
.products-content-block{
    text-align: center;
    margin-right: 14.25rem;
}
.products-content-block-headline{
    font-size: 2rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    color: #2ECC71;
    margin-bottom: 1.5rem;
}
.products-content-block-text{
    font-size: 1.375rem;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    margin-bottom: 5.69rem;
}
@media screen and (max-width: 361px){
    .products-headline{
        font-size: 2.1875rem;
        margin-bottom: 1.37rem;
    }
    .products-content-wrapper{
        margin-bottom: 1.87rem;
        flex-direction: column;
    }
    .products-content-block{
        margin-right: 0;
    }
    .products-content-block-headline{
        font-size: 1.5625rem;
    }
    .products-content-block-text{
        font-size: 1.125rem;
    }
}
</style>