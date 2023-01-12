<template>
    <div class="container-fluid text-center project">
        <div class="row">
            <div class="col rounded-3">
                <h1 class="display-5 Shinobi text-light text-shad-white mx-3 my-3 kage animated-charcter fw-bolder">|Projects|</h1>
            </div>
        </div>
        <div data-aos="fade-up" data-aos-duration="700" id="skills" class="container text-center">
            <hr class="w-50 mx-auto pb-5">
          </div>
          <div class="card-holder row d-flex justify-content-around mx-auto g-4">
            <div class="card col-4 col-md-6" style="width: 18rem" v-for="project in projects" :key="project">
              <img :src="project.img" class="card-img-top img-fluid" alt="" />
              <div class="card-body">
                <h5 class="card-title" v-text="project.brand"></h5>
                <p class="card-text" v-text="project.model"></p>
                <a :href="project.github">Github Link</a>
                <br>
                <a :href="project.netlify">Netlify Link</a>
              </div>
            </div>
          </div>
    </div>
</template>
<script>
export default {
  data() {
    return {
      projects: [
        {
          id: "1",
          brand: "Portfolio",
          model: "Project1",
          img: "https://i.postimg.cc/NfZf4cx2/Portfolio-Project-1.jpg",
          github:"https://github.com/MatthewJesseThomas/Portfolio-.git",
          netlify:"https://matthewjessethomas22.netlify.app/",
        },
        {
          id: "2",
          brand: "Ghost-Gaming",
          model: "Project2",
          img: "https://i.postimg.cc/d0WJ3w2c/Screenshot-2022-10-31-141908.jpg",
          github:"https://github.com/MatthewJesseThomas/exercise",
          netlify:"https://matthewjessethomas22.netlify.app/",
        },
        {
          id: "3",
          brand: "Abstract Gaming",
          model: "Project3",
          img: "https://screenshot-proxy.netlify.app/f_webp,w_336/https://d33wubrfki0l68.cloudfront.net/634d6b0fb298de00097b01d7/screenshot_2022-10-17-14-47-51-0000.png",
          github:"https://github.com/MatthewJesseThomas/Portfolio-.git",
          netlify:"https://abstractgaming.netlify.app",
        },
        {
          id: "4",
          brand: "Calculator",
          model: "Project4",
          img: "https://screenshot-proxy.netlify.app/f_avif,w_336/https://d33wubrfki0l68.cloudfront.net/637f14011f56592ca68789a9/screenshot_2022-11-24-06-49-42-0000.png",
          github:"https://github.com/MatthewJesseThomas/JavaScript-Calculator.git",
          netlify:"https://my-javascript-calculator-task.netlify.app",
        },
        {
          id: "5",
          brand: "Stygian Umbra Gaming",
          model: "Project5",
          img: "https://screenshot-proxy.netlify.app/f_avif,w_336/https://d33wubrfki0l68.cloudfront.net/639c601a39cc2c0069ecef5a/screenshot_2022-12-16-12-10-08-0000.png",
          github:"https://github.com/MatthewJesseThomas/EOMP-JAVASCRIPT.git",
          netlify:"https://stygian-umbra-gaming.netlify.app",
        },
        {
          id: "6",
          brand: "Ghost-Gaming",
          model: "Project6",
          img: "https://screenshot-proxy.netlify.app/f_avif,w_336/https://d33wubrfki0l68.cloudfront.net/63bfeeb93dbee200b494cdd5/screenshot_2023-01-12-11-27-59-0000.png",
          github:"https://github.com/MatthewJesseThomas/JS-Random-PassWord-Generator.git",
          netlify:"https://random-password-generator-javascript.netlify.app/",
        }
      ],
    };
  },
};

</script>
<style>
.project{
    margin-top: 8rem;
}   
</style>