<template >
    <div class="test">
        <h1 class="animated-charcter text-light">Testimonials</h1>
        <br>
        <h2 class="animated-charcter text-light">•As Follows•</h2>
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
.test{
    margin-top: 9rem;
}    
</style>