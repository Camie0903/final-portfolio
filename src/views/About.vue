<template>
    <div class="Ab_head">
       <h1>About me</h1>
    </div>
    <div class="row">
      <div class="column">
        <div class="img_abt">
          <img
                  class="img-fluid"
                  id="ap"
                  src="https://i.postimg.cc/PJm8KQZF/Cameron-1.jpg"
                />
        </div>
        <div class="abt_para1">
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
<style>
.Ab_head{
  margin-top: -13%;
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
}
#ap{
     width: 470px;
    height: 500px;
    display: flex;
   float: left;
}
.fir_para{
  margin-top:5%;
}
.sec_para{
  margin-top:5%;
}
.abt_para1{
  display: flex;
  flex-wrap: wrap; 
  margin-left: 50%;
  /* margin-top: 50%; */
  margin-top: 6%;
  margin-right: 10%;
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