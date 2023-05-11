<template>
    <div id="timeline-content whole_content">
  <div class>
    <h1 data-shadow='Resume'>Resume</h1>
  </div>
  <ul class="timeline">
    <li class="event" data-date="2015-2020">
      <h3>Voortrekker High School</h3>
      <p>I matriculated at Voortrekker High in Kenilworth, and that was where I found my passion for Web Development.</p>
    </li>
    <li class="event" data-date="2021">
      <h3>CartRun</h3>
      <p>I was an instore shopper for people that couldn't make it to go to shops during COVID19.</p>    
    </li> 
     <li class="event" data-date="2021">
      
      <h3>CTU Training Solutions</h3>
      
      <p>At CTU Training Solutions I studied Information Systems for a year. </p>
    </li> 
    <li class="event" data-date="2022">
      
      <h3>Life Choices Academy</h3>
      
      <p>At Life Choices I found my strengths and weaknesses in coding, and today I can say it was a very wise and good choice to study at Life Choices.</p>
    </li>
    <li class="event" data-date="Oct 22-Apr 23">
      
      <h3>Webwiser</h3>
      
      <p> At WebWiser, a reputable web development company, I had the opportunity to work as a Junior Web Developer on several high-profile projects for well-known brands such as Crocs, Under Armour, and Birkenstock. My role involved working closely with senior developers to create responsive and visually appealing websites that met the clients' requirements.</p>
    </li>
  </ul>
</div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
@import url(https://fonts.googleapis.com/css?family=Righteous);

/* .res_head {
  margin-top: -13%;
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
} */

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

body {
  background: #252827;
  font-size: 16px;
}

p {
  font-weight: 300;
}

a {
  color: #6c6d6d;
  text-decoration: none;
  text-transform: uppercase;
  display: block;
  letter-spacing: 0.3em;
  font-size: 0.6em;
  font-weight: 400;
  background: #252727;
  padding: 0.3rem 1rem;
  margin: 1.9rem 0 0 0;
  float: right;
}

a:hover {
  color: white;
  background: #004ffc;
  border-bottom: 0.35em solid black;
}

strong {
  font-weight: 600;
}

h1 {
  letter-spacing: 1.5px;
  color: white;
  font-weight: 400;
  color: white;
  font-family: "Righteous", serif;
  font-size: 5.5rem;
  text-shadow: 0.03em 0.03em 0 hsla(230, 40%, 50%, 1);
  padding-top: 5rem;
  position: relative;
}

/* h1:after {
  position: absolute;
  content: attr(data-shadow);
  top: 0.02em;
  left: 0.1em;
  z-index: -1;
  text-shadow: none;
  
  background-image: linear-gradient(
    45deg,
    transparent 45%,
    hsla(48, 20%, 90%, 1) 45%,
    hsla(48, 20%, 90%, 1) 55%,
    transparent 0
  );
  background-size: 0.02em 0.05em;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;

  animation: shad-anim 15s linear infinite;
} */

@keyframes shad-anim {
  0% {
    background-position: 0 0;
  }
  0% {
    background-position: 100% -100%;
  }
}

#timeline-content {
  text-align: center;
}
/* Timeline */
.timeline {
  border-left: 4px solid #004ffc;
  border-bottom-right-radius: 4px;
  border-top-right-radius: 4px;
  background: rgba(255, 255, 255, 0.03);
  color: rgba(255, 255, 255, 0.8);
  font-family: 'Chivo', sans-serif;
  margin: 50px auto;
  letter-spacing: 0.5px;
  position: relative;
  line-height: 1.4em;
  font-size: 1.03em;
  padding: 50px;
  list-style: none;
  text-align: left;
  font-weight: 100;
  max-width: 50%;
}
.timeline h1 {
  font-family: 'Saira', sans-serif;
  letter-spacing: 1.5px;
  font-weight: 100;
  font-size: 1.4em;
}
.timeline h2,
.timeline h3 {
  font-family: 'Saira', sans-serif;
  letter-spacing: 1.5px;
  font-weight: 400;
  font-size: 1.4em;
}
.timeline .event {
  border-bottom: 1px dashed rgba(255, 255, 255, 0.1);
  padding-bottom: 25px;
  margin-bottom: 50px;
  position: relative;
}
.timeline .event:last-of-type {
  padding-bottom: 0;
  margin-bottom: 0;
  border: none;
}
.timeline .event:before,
.timeline .event:after {
  position: absolute;
  display: block;
  top: 0;
}
.timeline .event:before {
  left: -217.5px;
  color: rgba(255, 255, 255, 0.4);
  content: attr(data-date);
  text-align: right;
  font-weight: 100;
  font-size: 0.9em;
  min-width: 120px;
  font-family: 'Saira', sans-serif;
}
.timeline .event:after {
  box-shadow: 0 0 0 4px #004ffc;
  left: -57.85px;
  background: #313534;
  border-radius: 50%;
  height: 11px;
  width: 11px;
  content: "";
  top: 5px;
}
@media (min-width: 992px) {
  h1{
    padding-top: 0;
  }
  
}

</style>