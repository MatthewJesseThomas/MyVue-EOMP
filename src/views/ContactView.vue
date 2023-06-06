<template>
    <h1 class="text-light testimonial-heading">Contact Me</h1>
    <div class="my-3 d-flex align-items-center justify-content-center">
        <ContactForm/>
    </div>
</template>
<script>
import ContactForm from '../components/ContactForm.vue'
export default {
    components: {
        ContactForm
    }
};
</script>
<style lang="scss" scoped>
.testimonial-heading{
    font-size: 5rem;
    margin-bottom: 4rem;
}
</style>