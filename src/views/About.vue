<template>
  <div class="whole_content row mb-5">
    <h1 class="heading" data-attr-text="About Me">About Me</h1>
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
        <p class="third_para font-weight-bold">TechStack: HTML5, CSS, Node.js, Vue.js, Bootstrap, MySQL, JavaScript, TypeScript, Shopify, Tailwind CSS, React.js, Liquid and Vercel</p>
      </div>
      <div class="links">
        <div class="link">
          <a href="https://www.linkedin.com/in/cameron-tamboer-729b7a239/" target="_blank"><img src="https://i.postimg.cc/m2mg2Hjm/linkedin.png" class="contact_images" alt="linkedin"></a>
        </div>
        <div class="link">
          <a href="https://github.com/Camie0903" target="_blank"><img src="https://i.postimg.cc/YCV2QBJg/github.png" class="contact_images" alt="github"></a>
        </div>
        <div class="link">
          <a href="https://app.netlify.com/teams/camie0903/overview" target="_blank"><img src="https://i.postimg.cc/v82N8XfN/netlify-logo-png-transparent.png" class="contact_images" alt="netlify"></a>
        </div>
        <div class="link">
          <a href="mailto:camerontamboer03@gmail.com" target="_blank"><img src="https://i.postimg.cc/NjLfyjPB/email.png" class="contact_images" alt="email"></a>
        </div>
        <div class="link whatsapp_link">
          <a href="https://wa.me/+27677051854?text=Hey%20there!%20Just%20checking%20out%20your%20web%20developer%20portfolio%20and%20I'm%20really%20impressed%20with%20your%20work.%20Your%20designs%20are%20sleek%20and%20your%20code%20is%20clean.%20Would%20love%20to%20chat%20more%20about%20your%20process%20and%20experience.%20Let%20me%20know%20when%20you're%20free%20to%20chat!" target="_blank"><i class="fa-brands fa-whatsapp fa-2xl" style="color: #638ed9;"></i></a>
        </div>
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
     #contact {
/*   background-color: #2c3e50; */
  display: flex;
  justify-content: center;
  align-items: center;
}
.whatsapp_link{
  padding-top: 0.5rem;
    /* gap: 1rem; */
    padding-left: 0.5rem;
}
.contact-box {
  /* width: clamp(100px, 90%, 1000px); */
  width: 64%;
  margin: 80px 50px;
  margin-top: 30vh;
  display: flex;
  flex-wrap: wrap;
  margin-left: 34%;
    padding-top: 8rem;
}

.contact-links, .contact-form-wrapper {
  width: 50%;
  padding: 8% 5% 10% 5%;
}




.contact-form-wrapper {
  background-color: #ffffff8f;
  border-radius: 0 10px 10px 0;
  margin-top: -15%;
}

@media only screen and (max-width: 800px) {
  .contact-links, .contact-form-wrapper {
    width: 100%;
  }
  
  .contact-links {
    border-radius: 10px 10px 0 0;
  }
  
  .contact-form-wrapper {
    border-radius: 0 0 10px 10px;
  }
}

@media only screen and (max-width: 400px) {
  .contact-box {
    width: 95%;
    margin: 8% 5%;
  }
}

h2 {
  font-family: 'Arimo', sans-serif;
  color: #fff;
  font-size: clamp(30px, 6vw, 60px);
  letter-spacing: 2px;
  text-align: center;
  transform: scale(.95, 1);
}

.links {
  display: flex;
  flex-wrap: wrap;
  /* padding-top: 50px; */
  width: 470px;
  height: 500px;
  display: flex;
 float: left;
 padding-left: 6rem;
}
@media (max-width:729px) {
  .links{
    padding-left: 3rem;
    display: flex;
    flex-wrap: nowrap;
  }
  .abt_para1{
    padding-top:2rem;
  }
}
@media (max-width:964px) {
  .heading{
    padding-top: 5rem;
  }
  
}
.link {
  margin: 10px;
  cursor: pointer;
  
}
a{
    background: transparent;
}

.contact_images {
  width: 45px;
  height: 45px;
  filter: 
    hue-rotate(220deg)
    drop-shadow(2px 4px 4px #0006);
  transition: 0.2s;
  user-select: none;
}

.contact_images:hover {
  transform: scale(1.1, 1.1);
}

.contact_images:active {
  transform: scale(1.1, 1.1);
  filter: 
    hue-rotate(220deg)
    drop-shadow(2px 4px 4px #222)
    sepia(0.3);
}

.form-item {
  position: relative;
}

label, input, textarea {
  font-family: 'Poppins', sans-serif;
}

label {
  position: absolute;
  top: 10px;
  left: 2%;
  color: #999;
  font-size: clamp(14px, 1.5vw, 18px);
  pointer-events: none;
  user-select: none;
}

input, textarea {
  width: 100%;
  outline: 0;
  border: 1px solid #ccc;
  border-radius: 4px;
  margin-bottom: 20px;
  padding: 12px;
  font-size: clamp(15px, 1.5vw, 18px);
}

input:focus+label, 
input:valid+label, 
textarea:focus+label, 
textarea:valid+label {
  font-size: clamp(13px, 1.3vw, 16px);
  color: #777;
  top: -20px;
  transition: all .225s ease;
}

.submit-btn {
  background-color: #fd917e;
  filter: drop-shadow(2px 2px 3px #0003);
  color: #fff;
  font-family: "Poppins",sans-serif;
  font-size: clamp(16px, 1.6vw, 18px);
  display: block;
  padding: 12px 20px;
  margin: 2px auto;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  user-select: none;
  transition: 0.2s;
}

.submit-btn:hover {
  transform: scale(1.1, 1.1);
}

.submit-btn:active {
  transform: scale(1.1, 1.1);
  filter: sepia(0.5);
}

@media only screen and (max-width: 800px) {
  h2 {
    font-size: clamp(40px, 10vw, 60px);
  }
}

@media only screen and (max-width: 400px) {
  h2 {
    font-size: clamp(30px, 12vw, 60px);
  }
  
  .links {
    padding-top: 30px;
  }
  
  .contact_images {
    width: 38px;
    height: 38px;
  }
}
@media (max-width: 992px) {
  .contact-box{
    width:100%;
    display: flex;
    justify-items: center;
    align-items: center;
    justify-content: center;
    padding-right: 5rem;
    margin-top: 11rem;
    margin-left: 3rem;
  }
}
.whole_content{
  /* padding-left: 14rem;
    padding-right: 2rem; */
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

#ap {
  background-color: #F5F5F5; /* slight greyish background */
  width: 470px;
  height: 500px;
  display: flex;
  float: left;
  border-radius: 10px; /* adds rounded corners */
 
}
#ap:hover {
  transform: scale(1.05);
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.3); /* adds a subtle shadow */
}

.fir_para{
  margin-top: -10%;
}
.sec_para{
margin-top:5%;
}
.third_para{
margin-top:5%;
font-weight: 600;
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

@media  (max-width: 1180px) {
  .whole_content {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0;
  }
  /* .column {
    flex-direction: column;
  } */
  .img_abt {
    margin-bottom: 2rem;
  }
  .abt_para1 {
    margin-top: 2rem;
  }
}

@media (max-width: 480px) {
  .whole_content{
    padding-top: 5rem;
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