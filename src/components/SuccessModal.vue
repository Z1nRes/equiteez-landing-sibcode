<template>
    <div class="success-modal d-flex align-items-center justify-content-center">
        <p class="success-modal-text">Successfully! We will send early access soon.</p>
    </div>
</template>

<script>
export default {
    name: 'SuccessModal',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.success-modal{
    border-radius: 0.625rem;
    width: 36.25rem;
    height: 13.5rem;
    background-color: #fff;
}
.success-modal-text{
    margin: 0;
    padding: 0;
    text-align: center;
    font-size: 1.25rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
@media screen and (max-width: 361px){
    .success-modal{
        width: 18.25rem;
    }
}
</style>