<template>
    <div class="contact-box">
    <div class="contact-links">
      <h2>CONTACT ME...</h2>
      <div class="links">
        <div class="link">
          <a href="https://www.linkedin.com/in/cameron-tamboer-729b7a239/" target="_blank"><img src="https://i.postimg.cc/m2mg2Hjm/linkedin.png" alt="linkedin"></a>
        </div>
        <div class="link">
          <a href="https://github.com/Camie0903" target="_blank"><img src="https://i.postimg.cc/YCV2QBJg/github.png" alt="github"></a>
        </div>
        <div class="link">
          <a href="https://app.netlify.com/teams/camie0903/overview" target="_blank"><img src="https://i.postimg.cc/v82N8XfN/netlify-logo-png-transparent.png" alt="netlify"></a>
        </div>
        <div class="link">
          <a href="mailto:camerontamboer03@gmail.com" target="_blank"><img src="https://i.postimg.cc/NjLfyjPB/email.png" alt="email"></a>
        </div>
        <div class="link whatsapp_link">
          <a href="https://wa.me/+27677051854?text=Hey%20there!%20Just%20checking%20out%20your%20web%20developer%20portfolio%20and%20I'm%20really%20impressed%20with%20your%20work.%20Your%20designs%20are%20sleek%20and%20your%20code%20is%20clean.%20Would%20love%20to%20chat%20more%20about%20your%20process%20and%20experience.%20Let%20me%20know%20when%20you're%20free%20to%20chat!" target="_blank"><i class="fa-brands fa-whatsapp fa-2xl" style="color: #638ed9;"></i></a>
        </div>
      </div>
    </div>
    
  </div>
</template>
<script>
export default {};
</script>
<style scoped>

* {
  margin: 0;
  box-sizing: border-box;
}

body {
  background-color: #2c3e50;
}

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


.contact-links {
  background-color: #2c3e50;
  background:
    radial-gradient(
      circle at 55% 92%, #426691 0 12%, transparent 12.2%
    ), 
    radial-gradient(
      circle at 94% 72%, #426691 0 10%, transparent 10.2%
    ), 
    radial-gradient(
      circle at 20% max(78%, 350px), #263a53 0 7%, transparent 7.2%
    ), 
    radial-gradient(
      circle at 0% 0%, #263a53 0 40%, transparent 40.2%
    ), 
    #1f2e43;
  border-radius: 10px 0 0 10px;
  margin-top: -15%;
  /* margin-left: 15%; */
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
  justify-content: center;
  padding-top: 50px;
}

.link {
  margin: 10px;
  cursor: pointer;
  
}
a{
    background: transparent;
}

img {
  width: 45px;
  height: 45px;
  filter: 
    hue-rotate(220deg)
    drop-shadow(2px 4px 4px #0006);
  transition: 0.2s;
  user-select: none;
}

img:hover {
  transform: scale(1.1, 1.1);
}

img:active {
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
  
  img {
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
</style>