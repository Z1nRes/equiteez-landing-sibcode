<template>
    <div class="contact d-flex">
        <div class="contact-content">
            <h2 class="contact-headline">Contact Us</h2>
            <div class="contact-text">
                <p>For inquiries regarding events, projects,<br/>collaborations, or general information.<br/><span class="contact-link">info@equiteez.com</span></p>
            </div>
        </div>
        <ContactForm @modalChange="modalChange" />
    </div>
</template>

<script>
import ContactForm from './ContactForm.vue'

export default {
    name: 'ContactUs',
    components: {
        ContactForm,
    },
    methods: {
        modalChange(data) {
            this.$emit('modalChange', data)
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.contact{
    padding: 5.06rem 0 2.75rem 0;
}
.contact-link{
    cursor: pointer;
    color: #2ECC71;
}
.contact-headline{
    font-size: 2.8125rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}
.contact-text{
    font-size: 1.25rem;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
.contact-content{
    margin-right: 11.56rem;
    margin-top: 2.19rem;
}
@media screen and (max-width: 361px){
    .contact{
        flex-direction: column;
    }
    .contact-headline{
        font-size: 2.1875rem;
    }
    .contact-text{
        font-size: 1.125rem;
    }
    .contact-content{
        margin-right: 0;
    }
}
</style>