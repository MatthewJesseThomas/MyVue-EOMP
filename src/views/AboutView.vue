<template>
  <div class="about animated-charcter">
    <h1 class="display-6 kage animated-charcter fw-bold text-light">About Me</h1> <br>
    <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible align-self-center content">
      <h1 class="display-6 text-decoration-underline kage animated-charcter fw-bold">Who Is Matthew:</h1> <br>
      <p class="lead display-6 kage animate-charcter fw-semibold">I am a Young South African male, with Aspirations of many Great deals and Strive for excellence and immense proficiency amongst all else an for my work. My passions are Engineering, Gaming, Gardening Music etc. I am the Eldest of Three kids an Always try to lead by Example for my Siblings as well as Community.</p> <br>
      <h2 class="display-6 text-decoration-underline kage animated-charcter fw-bold">What Motivates Matthew:</h2> <br>
      <p class="lead display-6 kage animate-charcter fw-semibold">Money is a major factor coming from a Poverty Stricken Community although that has never stopped or Detered my sense of hunger for Success or that of being Goal driven. After my Father's Death I've had to grow up very Fast and take on Responsibilities that were at the time out of my abilities but held Steadfast and Unwavered by Circumstance went for Excellence and now am and will always be motivated by this drive for the Best Life has to Offer.
      </p>
      <br>
  </div>
  </div>
</template>
<script>

export default {

}
</script>
<style scoped>
.about{
    margin-top: 9rem;
    }
    @import url("https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900");

    * {
      font-family: "Poppins", sans-serif;
    }
    
    body {
      display: flex;
      background: #000;
      min-height: 100vh;
      align-items: center;
      justify-content: center;
    }
    
    .content {
      position: relative;
    }
    
    .content p {
      color: #fff;
      position: relative;
      transform: translate(-0.5%, -0.5%);
    }
    
    .content p:nth-child(1) {
      color: transparent;
      -webkit-text-stroke: 2px #03a9f4;
    }
    
    .content p:nth-child(2) {
      color: #03a9f4;
      animation: animate 4s ease-in-out infinite;
    }
    
    @keyframes animate {
      0%,
      100% {
        clip-path: polygon(
          0% 45%,
          16% 44%,
          33% 50%,
          54% 60%,
          70% 61%,
          84% 59%,
          100% 52%,
          100% 100%,
          0% 100%
        );
      }
    
      50% {
        clip-path: polygon(
          0% 60%,
          15% 65%,
          34% 66%,
          51% 62%,
          67% 50%,
          84% 45%,
          100% 46%,
          100% 100%,
          0% 100%
        );
      }
    }
</style>