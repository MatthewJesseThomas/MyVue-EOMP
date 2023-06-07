<template>
  <div class="container-fluid text-center project">
    <div class="row">
      <div class="col rounded-3">
        <h1 class="display-5 Shinobi text-light text-shad-white mx-3 kage animated-charcter fw-bolder project-heading">Projects</h1>
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
          <div class="Link-Icons stylus">
            <a :href="project.github">
              <svg class="GithubLinkIcon" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
                <path fill="currentColor" d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5c.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34c-.46-1.16-1.11-1.47-1.11-1.47c-.91-.62.07-.6.07-.6c1 .07 1.53 1.03 1.53 1.03c.87 1.52 2.34 1.07 2.91.83c.09-.65.35-1.09.63-1.34c-2.22-.25-4.55-1.11-4.55-4.92c0-1.11.38-2 1.03-2.71c-.1-.25-.45-1.29.1-2.64c0 0 .84-.27 2.75 1.02c.79-.22 1.65-.33 2.5-.33c.85 0 1.71.11 2.5.33c1.91-1.29 2.75-1.02 2.75-1.02c.55 1.35.2 2.39.1 2.64c.65.71 1.03 1.6 1.03 2.71c0 3.82-2.34 4.66-4.57 4.91c.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2Z" />
              </svg>
            </a>
            <a :href="project.netlify">
              <svg class="NetlifyLinkIcon" xmlns="http://www.w3.org/2000/svg" width="256" height="256" viewBox="0 0 256 256">
                <g fill="none">
                  <rect width="256" height="256" fill="#242938" rx="60" />
                  <path fill="url(#skillIconsNetlifyDark0)" d="M0 48l128 160l128-160H0z" />
                </g>
              </svg>
            </a>
          </div>
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
          netlify:"https://ghost-gaming.netlify.app/",
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
          brand: "JS Random Password Gen",
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
    margin-top: 1rem;
} 
.project-heading{
  font-size: 5.5rem;
  font-weight: 700;
}
.Link-Icons{
  display: flex;
  margin: auto;
  justify-content: space-between;
  justify-content: space-around;
  align-items: center;
}
.GithubLinkIcon{
  height: 4rem;
  width: 8rem;
}  
.GithubLinkIcon:hover{
  scale: 1.2;
}
.NetlifyLinkIcon{
  height: 4rem;
  width: 8rem;
}  
.NetlifyLinkIcon:hover{
  scale: 1.2;
}
.card-img-top{
  height: 12rem;
  margin-top: 5px;
  margin-left: 1px;
}
.card:hover{
  scale: 1.03;
  box-shadow: .5vw .5vw .3vh black;
  -webkit-transition: all 1s ease;
  transition: all 1s ease;
}
.hr-line{
  color: rgb(125, 10, 10, 1);
}
</style>