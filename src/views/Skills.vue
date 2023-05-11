<template>

    
    
    <div class="row whole_content">
    <h1 class="heading" data-attr-text="Skills">Skills</h1>

    <div id="skills_cont" class="row mb-5">
        <div id="skills_icons" class="col-md-6">
            <div class="i1">
                <i class="fa-brands fa-html5"></i>
                
            </div>
            <div class="i2">
                <i class="fa-brands fa-css3-alt"></i>
            </div>
            <div class="i3">
                <i class="fa-brands fa-bootstrap"></i>
            </div>
            <div class="i4">
                <i class="fa-brands fa-js-square"></i>
            </div>
            <div class="i5">
                <i class="fa-brands fa-vuejs"></i>
            </div>
            <div class="i6">
                <i class="fa-brands fa-node-js"></i>
            </div>
        </div>
    <!-- Skills Bar -->
        <div id="skill_bar" class="col-md-6">
            <div class="skills">
                <div class="details">
                    <span>HTMLs</span>
                    <span>90%</span>
                </div>
                <div class="bar">
                <div id="html-bar"></div>
                </div>
            </div>
    
            <div class="skills">
                <div class="details">
                    <span>CSS</span>
                    <span>80%</span>
                </div>
                <div class="bar">
                <div id="css-bar"></div>
                </div>
            </div>
    
            <div class="skills">
                <div class="details">
                    <span>BOOTSTRAP</span>
                    <span>75%</span>
                </div>
                <div class="bar">
                <div id="bootstrap-bar"></div>
                </div>
            </div>
    
            <div class="skills">
                <div class="details">
                    <span>JS</span>
                    <span>78%</span>
                </div>
                <div class="bar">
                <div id="js-bar"></div>
                </div>
            </div>
    
            <div class="skills">
                <div class="details">
                    <span>VUE</span>
                    <span>20%</span>
                </div>
                <div class="bar">
                <div id="vue-bar"></div>
                </div>
            </div>
    
            <div class="skills">
                <div class="details">
                    <span>NODE</span>
                    <span>2%</span>
                </div>
                <div class="bar">
                <div id="node-bar"></div>
                </div>
            </div>
    
        </div>
</div>
</div>    
</template>
<script>
export default {
    
}
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css?  family=Lora:400,400i,700,700i");
/* .sk_head{
    margin-top:13vh;
    font-size: 2rem;
    letter-spacing: 3px;
    color: #2c3e50;
    text-transform: uppercase;
    width: 100%;
    text-align: center;
    -webkit-box-reflect: below 0.5px linear-gradient(transparent, #0008);
    line-height: 0.9em;
    outline: none;
    animation: animate 6000000s linear infinite;
}
@keyframes animate {
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
body{
  margin: 0;
  color: #fff;
  background-color: #112;
  font-family: sans-serif;
  font-size: 1rem;
  text-align: center;
  min-height: 100vh;
}




/* svg text {
  font-family: Lora;
  letter-spacing: 10px;
  stroke: #ffa5d8;
  font-size: 5.5rem;
  font-weight: 700;
  stroke-width: 1;
 
  animation: textAnimate 5s infinite alternate;
  
}

@keyframes textAnimate {
  0% {
    stroke-dasharray: 0 50%;
    stroke-dashoffset:  20%;
    fill:hsl(189, 68%, 75%)

  }
  
  100% {
    stroke-dasharray: 50% 0;
    stroke-dashoffstet: -20%;
    fill: hsla(189, 68%, 75%,0%)
  }
  
} */

#skills_cont{
    display:flex;
    justify-content: space-around;
}
#skills_icons{
    font-size:5rem;
    display:flex;
    flex-wrap: wrap;
    gap: 2rem;
}
.i1{
    margin:5%;
}
.i2{
    margin:5%;
}
.i3{
    margin:5%;
}
.i4{
    margin:5%;
}
.i5{
    margin:5%;
}
.i6{
    margin:5%;
}
.details{
    width: 100%;
    display: flex;  
    justify-content: space-between;
    margin-bottom: 10px;
}
/* #skill_bar{
    justify-content: stretch;
} */
#skill_bar{
    width: 600px;
}
.bar{
    /* position: relative; */
    /* border-radius: 20px; */
    width:100%;

}
.bar div{
    position: relative;
    width: 0;
    height: 9px;
    border-radius: 10px;
    background-color: #0d96e0;


}
.skills:not(:last-child){
    margin-bottom: 30px;
}
#html-bar{
    animation: html-fill 6s forwards;
}
@keyframes html-fill{
    100%{
        width: 90%;
    }
}
#css-bar{
    animation: css-fill 6s forwards;
}
@keyframes css-fill{
    100%{
        width: 80%;
    }
}
#bootstrap-bar{
    animation: bootstrap-fill 6s forwards;
}
@keyframes bootstrap-fill {
    100%{
        width: 75%;
    }
}
#js-bar{
    animation: js-fill 6s forwards;
}
@keyframes js-fill {
    100%{
        width: 78%;
    }
}
#vue-bar{
    animation: vue-fill 6s forwards;
}
@keyframes vue-fill {
    100%{
        width: 20%;
    }
}
#node-bar{
    animation: node-fill 6s forwards;
}
@keyframes node-fill {
    100%{
        width: 2%;
    }
}
@media (max-width: 480px) {
  .whole_content{
    padding-top: 5rem;
  }
  
}
</style>