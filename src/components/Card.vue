<template>
    <div class="col-11 col-sm-4 card bg-dark mx-3 my-3 TestimonialCard" style="width: 18rem;">
        <img :src="imgSrc" class="card-img-top" alt="Meh" loading="lazy">
        <div class="card-body">
          <h5 class="display-6 card-title kage animate-charcter fst-italic"> {{ name }} </h5>
          <h5 class="display-6 card-title kage animate-charcter fs-2 fst-italic"> {{ relation }} </h5>
          <p class="card-text kage animate-charcter fw-semibold">{{ quote }} </p>
        </div>
    </div>
</template>
<script>
export default {
    props: ['imgSrc', 'name', 'relation', 'quote']
}
</script>
<style>
.TestimonialCard:hover{
scale: 1.1;
box-shadow: .3vw .3vw 1vw #663399;

}
</style>