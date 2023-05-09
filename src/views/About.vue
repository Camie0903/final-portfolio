<template>

    <div class="patterns">
  <svg width="100%" height="100%">  
 <text x="50%" y="70%"  text-anchor="middle"  >
   About Me
 </text>
 </svg>
  </div>
  
  <div class="whole_content row mb-5">
    <div class="column row d-flex">
      <div class="col-md-6 img_abt d-flex justify-content-center">
        <img
                class="img-fluid"
                id="ap"
                src="https://i.postimg.cc/PJm8KQZF/Cameron-1.jpg"
              />
      </div>
      <div class="col-md-6 abt_para1 text-center">
        <p class="fir_para"> I am a South African freelance full stack developer. I am passionate about creating and maintaining websites, I have all the experience needed to create a responsive website. 
        I've spent 2 years in the coding industry, I found my passion through working with the coding language HTML and today i can say that I have learnt much more and I find coding much more intriguing, 
        everyday is something new to learn. All that I am and all I can do was all through practice.</p>
        <p class="sec_para">Since I've been coding I always lived up to this specific words of Steve Jobs, 
          <i>"People think focus means saying yes to the thing you've got to focus on. 
        It means saying no to the hundred other good ideas that there are. You have to pick carefully."</i></p>
      </div>
      <!-- <div class="abt_para1">
        Since I've been coding I always lived up to this specific words of Steve Jobs, <i>"People think focus means saying yes to the thing you've got to focus on. 
        It means saying no to the hundred other good ideas that there are. You have to pick carefully."</i>
      </div> -->
    </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped>
     @import url("https://fonts.googleapis.com/css?  family=Lora:400,400i,700,700i");

.whole_content{
  padding-left: 14rem;
    padding-right: 2rem;
}
.patterns{
  padding-top: 5rem;
  padding-left:6rem;
}


svg text {
  font-family: Lora;
  letter-spacing: 10px;
  stroke: #ffa5d8;
  font-size: 150px;
  font-weight: 700;
  stroke-width: 3;
 
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
  
}



/* .Ab_head{
margin-top: 5vh;
margin-bottom:14vh ;
font-size: 2.4rem;
font-weight: 400;
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
#ap{
background-color: black;
   width: 470px;
  height: 500px;
  display: flex;
 float: left;
}
.fir_para{
  margin-top: -10%;
}
.sec_para{
margin-top:5%;
}
.abt_para1{

display: flex;
flex-wrap: wrap; 
/* width:100%; */
/* margin-top: 50%; */
margin-top: 6%;

/* float: right; */
}
/* .abt_para2{
 display: flex;
flex-wrap: wrap;
margin-left: 50%;
/* margin-top: -10%; */
/* margin: 10%; */
/* float: right; */
i:hover {
  color: cadetblue;
  box-shadow: rgb(0 0 0 / 35%) 0px 5px 15px;
  border-radius: 10px;
  padding: 10px;
  transition: ease;
}    
</style>