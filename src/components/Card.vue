<template>
    <div class="col-11 col-sm-4 card bg-dark mx-3 my-3" style="width: 18rem;">
        <img :src="imgSrc" class="card-img-top" alt="Meh" loading="lazy">
        <div class="card-body">
          <h6 class="display-6 card-title kage animate-charcter fw-bold"> {{ name }} <br>{{ relation }} </h6>
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
    
</style>