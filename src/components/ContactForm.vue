<template>
    <div class="contact-form">
        <form class="form d-flex flex-column align-items-end">
            <div class="form-items-wrapper d-flex flex-column">
                <div class="form-item d-flex justify-content-between"> 
                    <label class="form-input-label" for="name">Name</label>
                    <input type="text" name="name" class="form-input form-control"/>
                </div>
                <div class="form-item d-flex justify-content-between"> 
                    <label class="form-input-label" for="company">Company</label>
                    <input type="text" name="company" class="form-input form-control"/>
                </div>
                <div class="form-item d-flex justify-content-between"> 
                    <label class="form-input-label" for="email">E-mail*</label>
                    <input type="email" name="email" required class="form-input form-control" />
                </div>
                <div class="form-item d-flex justify-content-between"> 
                    <label class="form-input-label" for="msg">Message*</label>
                    <textarea name="msg" required class="form-input form-input-area form-control"></textarea>
                </div>
            </div>
            <div>
                <button class="form-btn btn btn-dark" @click="modalChange">Send</button>
            </div>
        </form>
    </div>
</template>

<script>
    export default {
        name: 'ContactForm',
        methods: {
            modalChange() {
                this.$emit('modalChange', {isModal: true, success: true, form: false})
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.form-control{
    border: 1px solid #969696;
}
.form-item{
    width: 40.8125rem;
}
.form-item:not(:last-child){
    margin-bottom: 1.25rem;
}
.form-input{
    width: 33.75rem;
    background-color: transparent !important;
}
.form-input-label{
    font-size: 1.25rem;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
.form-input-area{
    background-color: transparent !important;
    resize: none;
    height: 8.25rem;
}
.form-btn{
    margin-top: 1.69rem;
    width: 10rem;
    border: 2px solid #252525;
    background-color: #252525;
}
.form-btn:hover{
    background-color: transparent !important;
    color: #252525;
}
@media screen and (max-width: 361px){
    .form{
        align-items: start !important;
    }
    .form-item{
        flex-direction: column;
        width: 20rem;
    }
    .form-input{
        width: 20rem;
    }
    .form-btn{
        width: 20rem;
    }
}
</style>