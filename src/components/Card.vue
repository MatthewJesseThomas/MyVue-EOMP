<template>
    <div class="col-11 col-sm-6 col-md-4 card testimonial-card">
      <div class="testimonial-card-inner">
        <div class="testimonial-card-front">
          <img :src="imgSrc" class="card-img-top" alt="Meh" loading="lazy">
          <div class="card-body">
            <h5 class="display-6 card-title name animate-character fst-italic">{{ name }}</h5>
            <h5 class="display-6 card-title relation animate-character fs-2 fst-italic">{{ relation }}</h5>
            <p class="card-text quote animate-character fw-semibold">{{ quote }}</p>
          </div>
        </div>
        <div class="testimonial-card-back">
          <h5 class="display-6 card-title name fst-italic">{{ name }}</h5>
          <h5 class="display-6 card-title relation fs-2 fst-italic">{{ relation }}</h5>
          <p class="card-text quote fw-semibold">{{ quote }}</p>
        </div>
      </div>
    </div>
  </template>
    
  <script>
  export default {
    props: ['imgSrc', 'name', 'relation', 'quote']
  }
  </script>
    
  <style>
  .testimonial-card {
    position: relative;
    perspective: 1000px;
    border: none;
    background-color: transparent;
  }
  
  .testimonial-card-inner {
    position: relative;
    width: 100%;
    height: 0;
    padding-top: 100%;
    transition: transform 0.5s;
    transform-style: preserve-3d;
  }
  
  .testimonial-card:hover .testimonial-card-inner {
    transform: rotateY(180deg);
  }
  
  .testimonial-card-front,
  .testimonial-card-back {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
  }
  
  .testimonial-card-front {
    z-index: 2;
    transform: rotateY(0deg);
  }
  
  .testimonial-card-back {
    transform: rotateY(180deg);
    background-color: #663399;
    color: #fff;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 20px;
  }
  
  .card-img-top {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 4px;
    margin-bottom: 10px;
  }
  
  .card-body {
    padding: 20px;
  }
  
  .name {
    animation: slideInLeft 0.5s forwards;
  }
  
  .relation {
    animation: slideInRight 0.5s forwards;
  }
  
  .quote {
    animation: fadeIn 0.5s forwards;
  }
  
  @keyframes slideInLeft {
    from {
      transform: translateX(-100%);
      opacity: 0;
    }
    to {
      transform: translateX(0);
      opacity: 1;
    }
  }
  
  @keyframes slideInRight {
    from {
      transform: translateX(100%);
      opacity: 0;
    }
    to {
      transform: translateX(0);
      opacity: 1;
    }
  }
  
  @keyframes fadeIn {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }
  
  @media (max-width: 767px) {
    .testimonial-card {
      margin-bottom: 20px;
    }
  }
  </style>
  