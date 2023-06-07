<template>
  <div class="myCards">
    <div
      class="row text-light rounded-3 py-5"
      data-aos="flip-right"
      data-aos-easing="ease-out-cubic"
      data-aos-duration="2000"
    >
      <div class="row d-flex justify-content-around mx-auto">
        <Card
          imgSrc="https://i.postimg.cc/BvmPdL9L/Profile-Pic6.jpg"
          name="John-Bruce Noad"
          relation="Colleague"
          quote="Matthew is Highly resourceful and a go-getting colleague, I have full trust in his ability to work in and under Pressure well, with his apparent sense of Leadership I never feel lost."
        />
        <Card
          imgSrc="https://i.postimg.cc/7ZFPwC2t/Joel-Profile.jpg"
          name="Joel Mukanya"
          relation="Lecturer"
          quote="Matthew is a very creative and well-behaved student. He is very driven by knowledge, enjoys working with his classmates, and does well working on his project. He has learned many new tricks in web development and bootstrap 5. I am quite happy with the effort he puts into his work. I recommend him as a developer."
        />
        <Card
          imgSrc="https://i.postimg.cc/kX8XT5g3/profile-1.jpg"
          name="Camryn Herandien"
          relation="Colleague"
          quote="Matthew is Highly resourceful and a go-getting colleague, I have full trust in his ability to work in and under Pressure well, with his apparent sense of Leadership I never feel lost."
        />
      </div>
    </div>
    <div
      class="row text-light rounded-3 py-5"
      data-aos="flip-left"
      data-aos-easing="ease-out-cubic"
      data-aos-duration="2000"
    >
      <div class="row d-flex justify-content-around mx-auto">
        <Card
          imgSrc="https://i.postimg.cc/bv432NL5/Profile-Pic7.jpg"
          name="Faeez Miller"
          relation="Colleague"
          quote="Knowing Matthew as long as I do, I'm able to gauge his Drive for coding as well as his Personality on a Newly found level as we are from the same Area and for the both of Us to be Developing, I wish him well in all Endeavors."
        />
        <Card
          imgSrc="https://i.postimg.cc/xTqqW2Mx/candice-2022.jpg"
          name="CANDICE AMON"
          relation="LifeChoicesAcademy Facilitator"
          quote="He is a very interactive individual. Very respectful towards his peers and anyone he encounters. Has a great appetite to learn. Matthew is always ready for a challenge and willing to give his all to excel in what he does. One of his greatest strengths is that he is an awesome team player."
        />
        <Card
          imgSrc="https://i.postimg.cc/DwRqG00W/IMG-20221105-090125.jpg"
          name="Seth Kallis"
          relation="Colleague"
          quote="Matthew is a Multi-faceted Individual, whom I have come to know as a Take-Charge and Work-driven person. If anything working with him has made Him and I grow immensely."
        />
      </div>
    </div>
  </div>
</template>

<script>
import Card from "@/components/Card.vue";

export default {
  components: {
    Card,
  },
};
</script>

<style>
.myCards {
  display: flex;
  flex-direction: column;
  margin: auto;
  margin-top: 2rem;
  margin-bottom: 8rem;
  padding-left: 1rem;
  padding-right: 1rem;
  align-content: center;
  justify-content: space-between;
  justify-content: space-around;
}

.card-img-top {
  height: 18rem;
  width: 15rem;
  object-fit: cover;
  border-radius: 4px;
  margin-bottom: 10px;
}

.card-body {
  height: auto;
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
  .myCards {
    margin-bottom: 2rem;
    padding-left: 0;
    padding-right: 0;
  }

  .card-img-top {
    width: 100%;
    height: 250px;
  }

  .card-body {
    height: auto;
    padding: 10px;
  }

  .name {
    animation: none;
  }

  .relation {
    animation: none;
  }

  .quote {
    animation: none;
  }
}
</style>
