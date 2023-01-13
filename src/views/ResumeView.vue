<template>
<div class="container-fluid text-center resume">
    <div class="row">
        <div class="col rounded-3">
            <h1 class="display-5 Shinobi text-light mx-3 my-3 kage animated-charcter fw-bolder">|Resume|</h1>
        </div>
    </div>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible w-75 m-auto justify-content-center">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">|EDUCATION|</h1> <br>
                <h1 class="display-5 text-decoration-underline kage animate-charcter fw-bolder">Matriculated From:</h1> <br>
                <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">{{ resume[0].school }} </h2> <br>
                <p class="lead display-6 kage animate-charcter fw-semibold">Year Of Matriculation:{{ resume[0].matriculation }} </p> <br>
                <p class="lead display-6 kage animate-charcter fw-semibold">Matriculated With:Bachelors</p> <br>
            </div>
            <br>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible w-75 m-auto justify-content-center">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">|EDUCATION|</h1> <br>
                <h1 class="display-5 text-decoration-underline kage animate-charcter fw-bolder">{{ resume[1].typeOfEducation }}</h1> <br>
                <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">{{resume[1].school}}</h2> <br>
                <p class="lead display-5 kage animate-charcter fw-semibold">{{resume[1 ].attended}}</p> <br>
            </div>
            <br>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible w-75 m-auto justify-content-center">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">|EXPERIENCE:|</h1>
                <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">{{ resume[2].retail }} <br>{{ resume[2].when }} <br> {{ resume[2].fb }} <br> {{ resume[2].date }} <br> {{ resume[2].engineering }} <br> {{ resume[2].timeSpent }} <br> {{ resume[2].developer }} <br> {{ resume[2].timeFrame }} </h2>
            </div>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible w-75 m-auto justify-content-center">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">|Skills:|</h1>
                <h1>Card Flip with Text</h1>
                <h3>Hover over the image below:</h3>

                <div class="flip-card">
                <div class="flip-card-inner">
                    <div class="flip-card-front">
                    <img src="https://i.postimg.cc/2jH1QjDN/html-png.png" alt="Avatar" style="width:300px;height:300px;">
                    </div>
                    <div class="flip-card-back">
                    <h1>HTML</h1> 
                    <p>Competency</p> 
                    <p>Expert</p>
                    </div>
                </div>
                </div>
                <div class="flip-card">
                <div class="flip-card-inner">
                    <div class="flip-card-front">
                    <img src="https://i.postimg.cc/K8LGKxfb/pngegg-5.png" alt="Avatar" style="width:300px;height:300px;">
                    </div>
                    <div class="flip-card-back">
                    <h1>CSS</h1> 
                    <p>Competency</p> 
                    <p>Expert</p>
                    </div>
                </div>
                </div>
                <div class="flip-card">
                <div class="flip-card-inner">
                    <div class="flip-card-front">
                    <img src="https://i.postimg.cc/yNYbMTkG/bootstrap.png" alt="Avatar" style="width:300px;height:300px;">
                    </div>
                    <div class="flip-card-back">
                    <h1>Bootstrap</h1> 
                    <p>Competency</p> 
                    <p>Expert</p>
                    </div>
                </div>
                </div>
                <div class="flip-card">
                <div class="flip-card-inner">
                    <div class="flip-card-front">
                    <img src="https://i.postimg.cc/FRGs9pZJ/pngegg-3.png" alt="Avatar" style="width:300px;height:300px;">
                    </div>
                    <div class="flip-card-back">
                    <h1>JavaScript</h1> 
                    <p>Competency</p> 
                    <p>Expert</p>
                    </div>
                </div>
                </div>
                <div class="flip-card">
                <div class="flip-card-inner">
                    <div class="flip-card-front">
                    <img src="https://i.postimg.cc/j2KN1Mjw/pngegg-4.png" alt="Avatar" style="width:300px;height:300px;">
                    </div>
                    <div class="flip-card-back">
                    <h1>VUE-JS</h1> 
                    <p>Competency</p> 
                    <p>Expert</p>
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
.resume{
    margin-top: 8rem;
}
body {
    font-family: Arial, Helvetica, sans-serif;
  }
  
  .flip-card {
    background-color: transparent;
    width: 300px;
    height: 300px;
    perspective: 1000px;
  }
  
  .flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.6s;
    transform-style: preserve-3d;
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  }
  
  .flip-card:hover .flip-card-inner {
    transform: rotateY(180deg);
  }
  
  .flip-card-front, .flip-card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
  }
  
  .flip-card-front {
    background-color: #bbb;
    color: black;
  }
  
  .flip-card-back {
    background-color: #2980b9;
    color: white;
    transform: rotateY(180deg);
  }    
</style>