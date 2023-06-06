<template>
    <h1 class="text-white headingShadow animated-charcter fw-bolder resume-heading">Welcome To my Resume Page...</h1>
<section class="timeline-section">
	<div class="timeline-items">
		<div class="timeline-item">
			<h2 class="myWhite"> Secondary Education </h2>
			<div class="timeline-dot"></div>
			<div class="timeline-date">2012</div>
			<div class="timeline-content">
				<h2 class="myWhite">EDUCATION</h2>
				<h3>Matriculated From:</h3>
				<h4 class="text-white">{{ resume[0].school }}</h4>
				<h4 class="text-white">Year Of Matriculation: <br> {{ resume[0].matriculation }} </h4>
				<h4 class="text-white">Matriculated With: <br> Bachelors</h4>
			</div>
		</div>
		<div class="timeline-item">
			<h2 class="myWhite"> Tertiary Education </h2>
			<div class="timeline-dot"></div>
			<div class="timeline-date">2017</div>
			<div class="timeline-content">
				<h2 class="text-white">EDUCATION</h2>
				<h3>{{ resume[1].typeOfEducation }}</h3>
				<h4 class="text-white">{{resume[1].school}}</h4>
				<h4 class="text-white">{{resume[1 ].attended}}</h4>
			</div>
		</div>
		<div class="timeline-item">
				<h2 class="myWhite"> EXPERIENCE </h2>
			<div class="timeline-dot"></div>
			<div class="timeline-date">2017</div>
			<div class="timeline-content">
				<h3>EXPERIENCE:</h3>
				<h4 class="text-white">{{ resume[2].retail }} <br>{{ resume[2].when }} <br> {{ resume[2].fb }} <br> {{ resume[2].date }} <br> {{ resume[2].engineering }} <br> {{ resume[2].timeSpent }} <br> {{ resume[2].developer }} <br> {{ resume[2].timeFrame }} </h4>
			</div>
		</div>
		<div class="timeline-item">
                <h2 class="myWhite"> Skills </h2>
			<div class="timeline-dot"></div>
			<div class="timeline-date">2022</div>
			<div class="timeline-content">
				<h3>HTML5</h3>
				<h4 class="text-white">Coding Language:</h4>
				<h4 class="text-white">:Web Development:</h4>
				<h4 class="text-white">Ability To Design Web Pages.</h4>
			</div>
		</div>
		<div class="timeline-item">
			<div class="timeline-dot"></div>
			<div class="timeline-date">2022</div>
			<div class="timeline-content">
				<h3>CSS3</h3>
				<h4 class="text-white">Coding Language:</h4>
				<h4 class="text-white">:Web Development:</h4>
				<h4 class="text-white">Ability To Style Web Pages.</h4>
			</div>
		</div>
		<div class="timeline-item">
			<div class="timeline-dot"></div>
			<div class="timeline-date">2022</div>
			<div class="timeline-content">
				<h3>BootStrap5</h3>
				<h4 class="text-white">Coding Language:</h4>
				<h4 class="text-white">:Web Development:</h4>
				<h4 class="text-white">Ability To Develop and Style Web Pages.</h4>
			</div>
		</div>
		<div class="timeline-item">
			<div class="timeline-dot"></div>
			<div class="timeline-date">2022</div>
			<div class="timeline-content">
				<h3>JavaScript</h3>
				<h4 class="text-white">Coding Language:</h4>
				<h4 class="text-white">:Web Development:</h4>
				<h4 class="text-white">To Use Javascript to add Functionality to websites.</h4>
			</div>
		</div>
	</div>
	<button class="btn btn-outline-info btn-dark mt-4 CV text-dark-emphasis">
		<a href="https://drive.google.com/uc?export=download&id=1dA4Jq-ntZqZ7XSh9XTdWD46gg4f4EMyK">Download CV</a>
	</button>
	<!-- Begin: HubSpot Academy - SEO Badge -->
	<!-- <div class='academy-badge my-5'>
		<a href='https://app-eu1.hubspot.com/academy/achievements/z1335rkn/en/1/matthew-jesse-thomas/seo' title='SEO'>
		<img src='https://hubspot-credentials-na1.s3.amazonaws.com/prod/badges/user/24ea668361f34f4694a7164d0313eda2.png' />
		</a>
	</div> -->
	<!-- End: HubSpot Academy - SEO Badge -->
</section>
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
.resume-heading{
	font-size: 3.5rem;
	margin-top: 2rem;
	margin-bottom: 2rem;
}
.resume{
margin-top: 3rem;
}
body {
font-family: 'Poppins', 'Arial', 'Helvetica', 'sans-serif';
}
.timeline-section{
	background-color: #c7ced31a;
	min-height: 100vh;
	padding: 100px 15px;
}
.timeline-content:hover{
    scale: 1.1;
}
.timeline-items{
	max-width: 1000px;
	margin:auto;
	display: flex;
	flex-wrap: wrap;
	position: relative;
}
.timeline-items::before{
	content: '';
	position: absolute;
	width: 2px;
	height: 100%;
	background-color: #2f363e;
	left: calc(50% - 1px);
}
.timeline-item{
	margin-bottom: 40px;
	width: 100%;
	position: relative;
}
.timeline-item:last-child{
	margin-bottom: 0;
}
.timeline-item:nth-child(odd){
    padding-right: calc(50% + 30px);
	text-align: right;
}
.timeline-item:nth-child(even){
    padding-left: calc(50% + 30px);
}
.timeline-dot{
	height: 16px;
	width: 16px;
	background-color: #eaa023;
	position: absolute;
	left: calc(50% - 8px);
	border-radius: 50%;
	top:10px;
}
.timeline-date{
	font-size: 18px;
	color: #eaa023;
	margin:6px 0 15px;
}
.timeline-content{
    background-color: #2f363e;
	padding: 30px;
	border-radius: 5px;
}
.timeline-content h3{
    font-size: 20px;
	color: #ffffff;
	margin:0 0 10px;
	text-transform: capitalize;
	font-weight: 500;
}
.timeline-content p{
    color: #c8c8c8;
	font-size: 16px;
	font-weight: 300;
	line-height: 22px;
}
.academy-badge {
	position: relative;
	width: 100%;
	max-width: 300px; /* Adjust the width as needed */
	margin: 0 auto;
	animation: floating 5.5s ease-in-out infinite;
}

@keyframes floating {
	0%,
	100% {
		transform: translateY(0);
		box-shadow: none;
	}
	50% {
		transform: translateY(-10px);
		box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
	}
}

.academy-badge img {
	width: 100%;
	display: block;
}

.academy-badge:hover {
	animation-play-state: paused;
}

.academy-badge img:hover {
	/* Add shine effect on hover */
	background: linear-gradient(
		90deg,
		rgba(255, 255, 255, 0) 0%,
		rgba(255, 255, 255, 1) 50%,
		rgba(255, 255, 255, 0) 100%
	);
	background-size: 200% 100%;
	animation: shine 5.5s linear infinite;
}

@keyframes shine {
	to {
		background-position: -200% center;
	}
}
/* responsive */
@media(max-width: 767px){
	.timeline-items::before{
		left: 7px;
	}
	.timeline-item:nth-child(odd){
		padding-right: 0;
		text-align: left;
	}
	.timeline-item:nth-child(odd),
	.timeline-item:nth-child(even){
		padding-left: 37px;
	}
	.timeline-dot{
		left:0;
	}
}
.CV{
	width: 20rem;
	height: 5rem;
	border-radius: 3rem;
	color: #c8c8c8;
}
.CV:hover{
	scale: 1.08;
	color:#c8c8c8;
}
.myWhite{
	color: rgba(240, 248, 255, 0.929);
	text-shadow: .3vw .3vw .3vh rgba(25, 21, 21, 0.826);
}
.headingShadow{
	text-shadow: .3vw .3vw .3vh rgba(25, 21, 21, 0.826);
}
</style>