<template>
    <div id="timeline-content">
  <div class="res_head">
    <h1>Resume</h1>
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
  </ul>
</div>
</template>
<script>
export default {
    
}
</script>
<style scoped>

.res_head{
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
  font-family: 'Saira', sans-serif;
  letter-spacing: 1.5px;
  color: white;
  font-weight: 400;
  font-size: 2.4em;
}
#timeline-content {
  margin-top: 30vh;
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
  max-width: 30%;
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

</style>