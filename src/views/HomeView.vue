<template>
  <div class="home">
    <section class="container-fluid sect">
      <div class="wrapper text-center">
          <div class="rounded-3 animated-charcter" data-aos="fade-down">
              <h1 class="text-white kage display-6 fw-bolder">Portfolio Of Matthew Jesse Thomas</h1>
          </div>
          <figure>
              <div class="my-auto">
                <div class="img-fluids d-flex alert-danger flex-column flex-sm-row">
                    <img class="img-fluid my-5 resize image-round" data-aos="fade-right" src="https://i.postimg.cc/xTXJBTtq/Profile-Pic1.jpg" alt="Matthew profile" loading="lazy">
                    <div class="container" data-aos="flip-down">
                      <div class="row">
                        <div class="col-lg-8 offset-lg-2">
                          <div class="paragraph-container">
                            <p class="text-light align-self-center  justify-content-md-around fw-bolder">
                              Hello There, I am Matthew Jesse Thomas,
                              I'm inspired by the work I've done in Software Development in all its success, and not to mention my unique career path Choice.
                              I saw a recent article on managing Developers in the Software Industry and had to Commence. I've managed to accelerate my Developmental Process in Web & Software Development, which has contributed toward as much as 90% growth in as few as three months time.
                            </p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="img-fluids d-flex border-alert-danger flex-column flex-sm-row">
                    <img class="img-fluid my-5 resize2 image-rounded" data-aos="fade-right" src="https://i.postimg.cc/VkDNNx72/Profile-Pic4.jpg" alt="Matthew profile" loading="lazy">
                    <div class="container">
                      <div class="row">
                        <div class="col-lg-8 offset-lg-2">
                          <div class="paragraph-container">
                            <p class="text-light align-self-center my-5 mt-5 justify-content-md-around fw-bolder">
                              •Matthew Thomas•
                              <br>
                              Its Inspiring to be in the working Industry of Software Development. Success in a Software Development career is Somewhat of a Dream for mine.
                              As an Aspiring Developer in the Industry it Begins Now with me. Thus I've managed to Develop a 'Critical' way of thinking and handling 'Problems' in Web & Software Development, which has contributed towards a much needed sense of Confidence as well as a Mindset shift with a focus towards "Exponential" growth in the Near Future.
                            </p>
                          </div>
                        </div>
                      </div>
                    </div>                    
                  </div>
              </div>
          </figure>
      </div>
  </section>
  </div>
</template>
<script>
export default {
    components:{
    }
}
</script>
<style scoped>
.home{
    margin-top: 9rem;
}
.img-fluids {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .image-round {
    width: 100%;
    max-width: 400px; /* Adjust the maximum width as needed */
    height: auto;
    border-radius: 50%;
    animation: floatAnimation 2s ease-in-out infinite;
  }
  
  @keyframes floatAnimation {
    0%, 100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-10px);
    }
  }
  
  .resize {
    transition: transform 0.3s ease-in-out;
  }
  
  .resize:hover {
    transform: scale(1.1);
  }
  
  .img-fluids {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .image-rounded {
    width: 100%;
    max-width: 600px;
    height: auto;
    border-radius: 50%;
    animation: floatAnimation 2s ease-in-out infinite;
  }
  
  @keyframes floatAnimation {
    0%, 100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-10px);
    }
  }
  
.myText{
    margin-left: 2rem;
}
.resize{
    height: 22rem;
    width: 23rem;
}
.resize2{
    height: 23rem;
    width: 23rem;
}
.sizing{
    height: 23rem;
}
.sizings{
    height: 22rem;
}
p{
  font-size: 26px;
}
h1{
  font-size: 48px;
  margin-top: 10rem;
  color: rgba(255, 255, 255, 0.8); /* White text color with opacity */
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}
</style>