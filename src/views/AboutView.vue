<template>
  <h1 class="kage animated-character fw-bold text-light about-heading">About Me</h1>
  <div class="about animated-character">
    <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible align-self-center wrapper">
      <h2 class="display-6 text-decoration-underline kage animated-character fw-bold typing-demo">Who Is Matthew:</h2>
      <p class="lead kage animated-character fw-semibold paragraph-text w-75">I am a Young South African male, with Aspirations of many Great deals and Strive for excellence and immense proficiency amongst all else an for my work. My passions are Engineering, Gaming, Gardening Music etc. I am the Eldest of Three kids an Always try to lead by Example for my Siblings as well as Community.</p>
      <h2 class="display-6 text-decoration-underline kage animated-character fw-bold typing-demo">What Motivates Matthew:</h2>
      <p class="lead kage animated-character fw-semibold  paragraph-text w-75">Money is a major factor coming from a Poverty Stricken Community although that has never stopped or Detered my sense of hunger for Success or that of being Goal driven. After my Father's Death I've had to grow up very Fast and take on Responsibilities that were at the time out of my abilities but held Steadfast and Unwavered by Circumstance went for Excellence and now am and will always be motivated by this drive for the Best Life has to Offer.</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.wrapper {
  height: 80%;
  max-width: 80vw;
  display: grid;
  place-items: center;
  overflow: hidden; /* Add this line */
}

.typing-demo {
  max-width: 100%; /* Add this line */
  width: auto; /* Add this line */
  animation: typing 8s steps(70), blink .5s step-end infinite alternate;
  white-space: normal; /* Modify this line */
  overflow-wrap: break-word; /* Modify this line */
  border-right: none; /* Remove this line */
  font-family: monospace;
  font-size: 2em;
}

.about-heading{
  font-size: 4.3rem;
}
p {
  font-size: clamp(24px 16px);
}

h1, h2 {
  font-size: 5rem;
  color: rgba(255, 255, 255, 0.8); /* White text color with opacity */
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
  margin-top: 3rem; /* Adjust the margin-top value to move the element down */
}

.about {
  margin-top: 5rem;
  overflow: hidden; /* Add this line */
}

.wrapper {
  height: 80%;
  max-width: 80vw;
  display: grid;
  place-items: center;
}

.typing-demo {
  width: 28ch;
  animation: typing 2s steps(28), blink .5s step-end infinite alternate;
  white-space: nowrap;
  overflow: hidden;
  border-right: 3px solid;
  font-family: monospace;
  font-size: 2em;
}

.paragraph-text {
  font-size: 2em;
  overflow-wrap: break-word; /* Add this line */
}

@keyframes typing {
  from {
    width: 0;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}

/* Responsive Styles */
@media screen and (max-width: 768px) {
  /* Adjust properties for screens up to 768px width */
  .about {
    margin-top: 6rem;
  }
  .wrapper {
    height: auto;
  }
  .typing-demo {
    font-size: 1.5em;
  }
}

@media screen and (max-width: 520px) {
  /* Adjust properties for screens up to 520px width */
  h1, h2 {
    font-size: 3rem;
    margin-top: 2rem;
  }
  .about {
    margin-top: 4rem;
  }
  .typing-demo {
    font-size: 1.8em;
  }
}

@media screen and (max-width: 480px) {
  /* Adjust properties for screens up to 480px width */
  .about {
    margin-top: 3rem;
  }
  .typing-demo {
    font-size: 1.2em;
  }
}

@media screen and (min-width: 100px) and (max-width: 2000px) {
  /* Adjust properties for screens within the specified width range */
  h1 {
    font-size: 3rem;
    margin-top: 2rem;
  }
  h2 {
    font-size: 2.5rem;
    margin-top: 2rem;
  }
  .about {
    margin-top: 4rem;
  }
  .typing-demo {
    font-size: 1.8em;
  }
}
</style>
