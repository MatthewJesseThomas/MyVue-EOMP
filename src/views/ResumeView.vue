<template>
<div class="container-fluid text-center resume">
    <div class="row">
        <div class="col rounded-3">
            <h1 class="display-5 Shinobi text-light mx-3 my-3 kage animated-charcter fw-bolder">|Resume|</h1>
        </div>
    </div>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">|EDUCATION|</h1> <br>
                <h1 class="display-5 text-decoration-underline kage animate-charcter fw-bolder">Matriculated From:</h1> <br>
                <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">{{ resume[0].school }} </h2> <br>
                <p class="lead display-6 kage animate-charcter fw-semibold">Year Of Matriculation:{{ resume[0].matriculation }} </p> <br>
                <p class="lead display-6 kage animate-charcter fw-semibold">Matriculated With:Bachelors</p> <br>
            </div>
            <br>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">|EDUCATION|</h1> <br>
                <h1 class="display-5 text-decoration-underline kage animate-charcter fw-bolder">{{ resume[1].typeOfEducation }}</h1> <br>
                <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">{{resume[1].school}}</h2> <br>
                <p class="lead display-5 kage animate-charcter fw-semibold">{{resume[1 ].attended}}</p> <br>
            </div>
            <br>
            <div class="col-sm-4-4 text-white text-shadow-white rounded-3 py-5 bible">
                <h1 class="display-5 text-decoration-underline kage animated-charcter fw-bolder">|EXPERIENCE:|</h1>
                <h2 class="display-6 text-decoration-underline kage animate-charcter fw-bold">{{ resume[2].retail }} <br>{{ resume[2].when }} <br> {{ resume[2].fb }} <br> {{ resume[2].date }} <br> {{ resume[2].engineering }} <br> {{ resume[2].timeSpent }} <br> {{ resume[2].developer }} <br> {{ resume[2].timeFrame }} </h2>
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
</style>