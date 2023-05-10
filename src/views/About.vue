<template>

<h1 class="heading" data-attr-text="About Me">About Me</h1>
  
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
        <p class="fir_para">As a freelance full-stack developer based in South Africa, I possess a passion 
          for creating and maintaining websites, backed by extensive experience in the field. Over the 
          course of two years, I have honed my skills in coding, with HTML serving as my gateway to the 
          coding world. Since then, my interest in coding has only deepened, and I have continued to 
          acquire new knowledge and skills on a daily basis through practice and dedication.</p>
        <p class="sec_para">Throughout my coding journey, I have adopted a philosophy that aligns 
          with the wise words of Steve Jobs, namely that true focus requires saying "no" to many good 
          ideas and carefully selecting the most relevant and impactful areas of focus. I am committed 
          to delivering high-quality results and providing excellent service to my clients.</p>
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

@media only screen and (max-width: 1179px) {
  .whole_content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 0;
  }
  .column {
    flex-direction: column;
  }
  .img_abt {
    margin-bottom: 2rem;
  }
  .abt_para1 {
    margin-top: 2rem;
  }
}


@media only screen and (max-width: 768px) {
    .whole_content {
      padding-left: 0;
      padding-right: 0;
    }
    .patterns {
      padding-top: 2rem;
      padding-left: 2rem;
    }
    svg text {
      font-size: 80px;
      letter-spacing: 5px;
    }
    #ap {
      width: 100%;
      height: auto;
      margin: 0 auto;
      float: none;
    }
    .abt_para1 {
      margin-top: 2rem;
    }
  }

  /* Styles for screens smaller than 576px (mobile devices) */
  @media only screen and (max-width: 576px) {
    .patterns {
      padding-left: 1rem;
    }
    svg text {
      font-size: 60px;
      letter-spacing: 3px;
    }
    .fir_para, .sec_para {
      font-size: 16px;
    }
  }
</style>