<template >
    <div class="test">
        <h1 class="animated-charcter text-light testimonial-heading">Testimonials</h1>
        <Testimonial/>
    </div>
</template>
<script>
import Testimonial from '../components/Testimonial.vue'
export default {
    components: {
        Testimonial
    }
};
</script>
<style>
.testimonial-heading{
    font-size: 4.5rem;
}
.test{
    margin-top: 1rem;
}    
</style>