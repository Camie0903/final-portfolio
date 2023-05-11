<template>
<div id="cardz">
<div id="pro">
  <div class="pro_head">
    <h1 class="heading" data-attr-text="Projects">Projects</h1>
  </div>  
    <div class="flip-card" v-for="proj in projects"
          :key="proj.id">
        <div class="flip-card-inner">
            <div class="flip-card-front">
              <img
              class="img-fluid rounded border border-5 border-dark"
              v-bind:src="proj.imgURL"
              id="testpic"
              />
          </div>
        <div class="flip-card-back">
            <h5 class="proj_tit">{{ proj.Title }}</h5>
            <p>{{ proj.description }}</p>
            <p>{{ proj.TechStack }}</p>
            <!-- <p>{{ proj.imgURL }}</p> -->
            <a class="link_btn1" :href="proj.github" target="blank">
                <i class="fa-brands fa-github"></i>
            </a>
            <a class="link_btn2" :href="proj.netlify" target="blank">
                <i class="fa-solid fa-eye"></i>
            </a>


        </div>

      </div>
    </div>
  </div>
</div>
            
</template>
<script>
export default {
    data(){
      return {
        projects:[
        {
            id: 1,
            Title: "BMI Calculator",
            description:"In this project, I've created a BMI Calculator where it indicates fatness in your body.",
            TechStack: "HTML, CSS, JS",
            imgURL: "https://i.postimg.cc/pLShfMx0/bmi.jpg",
            Github: "https://github.com/Camie0903/BMI_CALC",
            Live: "https://rococo-mermaid-22bb49.netlify.app/"
        },

        {
            id: 2,
            Title: "Temperature Converter",
            description:"In this project, I've created a Temperature Converter where you can see what degrees it is in Fahrenheit or Celsius.",
            TechStack: "HTML, CSS, JS",            
            imgURL: "https://i.postimg.cc/7YVSTRfc/tc.jpg",
            Github: "https://github.com/Camie0903/Temp_Convert",
            Live: "https://courageous-dodol-ba926c.netlify.app/"
        },
        {
            id: 4,
            Title: "Mock Portfolio",
            description:"In this project, I've created a mock portfolio.",
            imgURL: "https://i.postimg.cc/QMn2NSQK/Screenshot-2022-07-20-093352.png",
            Github: "https://github.com/Camie0903/A_Portfolio",
            Live: "https://camerons-portfolio.netlify.app/"
        },
        {
            id: 3,
            Title: "Mock Portfolio2",
            description:"In this project, I've created a mock portfolio as well.",
            imgURL: "https://i.postimg.cc/PryTsWRY/Screenshot-2022-07-20-093654.png",
            Github: "https://github.com/Camie0903/Portfolio2",
            Live: "https://cameron-portfolio.netlify.app/"
        },
        {
            id: 5,
            Title: "Calculator",
            description:"In this project, I've created a fully functional calculator.",
            imgURL: "https://i.postimg.cc/rFL94Wgd/cal.jpg",
            Github: "https://github.com/Camie0903/calculator",
            Live: "https://scintillating-conkies-e99358.netlify.app/"
        },
        {
            id: 6,
            Title: "To-Do List",
            description:"In this project, I've created a To-Do List where you can add things you still need to do, or tick a task you completed.",
            imgURL: "https://i.postimg.cc/tgy3ZHzL/istockphoto-1285308242-170667a.jpg",
            Github: "https://github.com/Camie0903/ToDoList",
            Live: "https://extraordinary-swan-d588eb.netlify.app/"
        },
        {
            id: 7,
            Title: "Real Estate",
            description:"In this project, I've created a website where it displays different types of properties.",
            imgURL: "https://i.postimg.cc/x8BypNVZ/rs.jpg",
            Github: "https://github.com/Camie0903/Property",
            Live: "https://serene-moxie-ee4fdf.netlify.app/"
        }

    ]}
}
}


</script>
<style scoped>

h1 {
  letter-spacing: 1.5px;
  color: white;
  font-weight: 400;
  color: white;
  font-family: "Righteous", serif;
  font-size: 5.5rem;
  text-shadow: 0.03em 0.03em 0 hsla(230, 40%, 50%, 1);

  position: relative;
}

.pro_head{
  margin-top: -11%;
   }
/* @keyframes animate {
  100% {
    color: #2c3e50;
    text-shadow: none;
  }
  0% {
    color: #fff;
    text-shadow: 0 0 10px #03BCF4, 0 0 20px #03BCF4, 0 0 40px #03BCF4,
      0 0 80px #03BCF4, 0 0 160px #03BCF4;
 
}
} */
#cardz{
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    margin-top: 20vh;
}
/* .card-body {
    } */
.proj_tit{
  margin-top:15%;
}
.wordingfr{
    font-size: medium;
}
.wording{
    margin:8%;
  font-size: medium;
}
.flip-card {
    background-color: transparent;
    width: 300px;
    height: 300px;
    perspective: 1000px;
    display: flex;
    flex-direction: column;
    border-radius: 50%;
    float: left;
    margin:2%;
  /* flex-wrap: wrap; */
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
.link_btn1{
    margin-right: 35%;
 
}
.flip-card-front {
    background-color: #bbb;
  color: black;
  height:300px;
  width:300px;
}
.flip-card-front img {
 
  height:300px;
  width:300px;
  object-fit: cover;
}

.flip-card-back {
  background-color: #2c3e50;
  color: white;
  transform: rotateY(180deg);
 font-size: small;
 margin-top: 5%;
}
@media (max-width: 1022px) {
  .flip-card{
    display: flex;
    flex-wrap: wrap;
    align-content: center;
    justify-content: center;
  }
  .pro_head{
    padding:0;
  }
}
</style>