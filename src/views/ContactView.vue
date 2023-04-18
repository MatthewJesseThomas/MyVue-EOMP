<template>
    <div class="border">
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
<style>
.border{
    border: 10rem 10rem red solid !important;
}
</style>