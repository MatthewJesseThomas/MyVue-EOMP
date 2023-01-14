<template>
<div class="container-fluid text-center resume">
    <div class="row">
        <div class="col rounded-3">
            <h1 class="display-5 Shinobi text-light mx-3 my-3 kage animated-charcter fw-bolder">Resume</h1>
        </div>
    </div>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible w-75 m-auto justify-content-center">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">EDUCATION</h1> <br>
                <h1 class="display-5 text-decoration-underline kage animate-charcter fw-bolder">Matriculated From:</h1> <br>
                <h2 class="display-6 kage animate-charcter fw-bold">{{ resume[0].school }} </h2> <br>
                <p class="lead display-6 kage animate-charcter fw-semibold">Year Of Matriculation: <br> {{ resume[0].matriculation }} </p> <br>
                <p class="lead display-6 kage animate-charcter fw-semibold">Matriculated With: <br> Bachelors</p> <br>
            </div>
            <br>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible w-75 m-auto justify-content-center">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">EDUCATION</h1> <br>
                <h1 class="display-5 kage animate-charcter fw-bolder">{{ resume[1].typeOfEducation }}</h1> <br>
                <h2 class="display-6  kage animate-charcter fw-bold">{{resume[1].school}}</h2> <br>
                <p class="lead display-5 kage animate-charcter fw-semibold">{{resume[1 ].attended}}</p> <br>
            </div>
            <br>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible w-75 m-auto justify-content-center">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">|EXPERIENCE:|</h1>
                <h2 class="display-6 kage animate-charcter fw-bold">{{ resume[2].retail }} <br>{{ resume[2].when }} <br> {{ resume[2].fb }} <br> {{ resume[2].date }} <br> {{ resume[2].engineering }} <br> {{ resume[2].timeSpent }} <br> {{ resume[2].developer }} <br> {{ resume[2].timeFrame }} </h2>
            </div>
            <div class="container-fluid text-center">
                <div class="row">
                    <div class="col rounded-3" data-aos="fade-up">
                        <h1 class="display-5 Shinobi text-light text-shad-white mx-3 my-3 kage animated-charcter fw-bolder">|Skills|</h1>
                    </div>
                </div>
                    <!-- <div class="row"> -->
                        <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible" data-aos="fade-up-right">
                            <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">HTML5</h1> <br>
                            <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">Coding Language:</h2> <br>
                      <p class="lead display-5 text-decoration-underline kage animate-charcter fw-semibold">:Web Development:</p> <br>
                      <p class="lead display-5 text-decoration-underline kage animate-charcter fw-semibold">Able To Code Web Pages</p> <br>
    <!-- skillbar -->
                            <h4 class="display-5 text-decoration-underline kage animated-charcter fw-semibold" id="Skills">:Proggress•Bar:</h4>
                    <div class="skillbar text-light text-center text-nowrap">
                        <div class="HTML5 my-2 ms-2" data-skill="HTML5">HTML5</div>
                    </div>
                        </div>
                    <!-- </div> -->
                    <br>
                        <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible" data-aos="fade-up-left">
                            <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">CSS3</h1> <br>
                            <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">Coding Language:</h2> <br>
                            <p class="lead display-5 text-decoration-underline kage animate-charcter fw-semibold">:Web Development:</p> <br>
                            <p class="lead display-5 text-decoration-underline kage animate-charcter fw-semibold">Able To Style Web Pages</p> <br>
    <!-- skillbar -->
                          <h4 class="display-5 text-decoration-underline kage animated-charcter fw-semibold" id="Skills">:Proggress•Bar:</h4>
                            <div class="skillbar text-light text-center text-nowrap">
                        <div class="CSS my-2 ms-2" data-skill="CSS">CSS</div>
                    </div>
                        </div>
                        <br>
                        <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible" data-aos="fade-up-right">
                            <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">BootStrap5</h1> <br>
                            <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">Coding Language:</h2> <br>
                            <p class="lead display-5 text-decoration-underline kage animate-charcter fw-semibold">:Web Development:</p> <br>
                            <p class="lead display-5 text-decoration-underline kage animate-charcter fw-semibold">Able To Code & Style Web Pages</p> <br> 
    <!-- skillbar -->
                          <h4 class="display-5 text-decoration-underline kage animated-charcter fw-semibold" id="Skills">:Proggress•Bar:</h4>
                            <div class="skillbar text-light text-center text-nowrap">
                      <div class="Bootstrap my-2 ms-2" data-skill="Bootstrap">Bootstrap</div>
                    </div>
                        </div>
                        <br>
                        <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible" data-aos="fade-up-left">
                            <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">JavaScript</h1> <br>
                            <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">Coding Language</h2> <br>
                            <p class="lead display-5 text-decoration-underline kage animate-charcter fw-semibold">Web Development</p> <br>
                            <p class="lead display-5 text-decoration-underline kage animate-charcter fw-semibold">Able To Use Js for Page Functionality</p> <br>
    <!-- skillbar -->
                          <h4 class="display-5 text-decoration-underline kage animated-charcter fw-semibold" id="Skills">:Proggress•Bar:</h4>
                          <div class="skillbar text-light text-center text-nowrap">
                    <div class="JavaScript my-2 ms-2" data-skill="JavaScript">JavaScript</div>
                  </div>
                        </div>
                    </div>
            
</div>
</template>
<script>
export default {
    data() {
        return {
            resume: [
                {
                 school:'Westridge Secondary High School',
                 matriculation: 2017,
                 qualification:'Bachelors',
                },
                {
                 typeOfEducation:'Tertiary:',
                 school:'College Of Cape Town',
                 attended: '2020-2022',
                },
                {
                 retail:'Retail in Sales: ',
                 when:'2018-2019',
                 fb:'Food and Beverage: ',
                 date:'2020-2021',
                 engineering:'Mechanical Engineering: ',
                 timeSpent:'2021-2022',
                 developer:'LifeChoices Coding Academy: ',
                 timeFrame:'Currently',

                }
            ]
        }
    },
};
</script>
<style>
<!-- .resume{
margin-top: 8rem;
}
body {
font-family: Arial, Helvetica, sans-serif;
}
</style>