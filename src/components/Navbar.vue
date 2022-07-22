<template>
    <div>
        <nav class="navheading">
            <ul class="navlist">
                <li class="navNames">
                    <router-link to="/">Home</router-link> 
                </li> 
                <li>
                    <router-link to="/about">About</router-link>
                </li>
                <li>
                    <router-link to="/skills">Skills</router-link>
                </li>
                <li>
                    <router-link to="/resume">Resume</router-link> 
                </li>
                <li>
                    <router-link to="/projects">Projects</router-link> 
                </li>
                <li>
                    <router-link to="/testimonials">Testimonials</router-link> 
                </li>
                <li>
                    <router-link  to="/contact">Contact</router-link> 
                </li>
            </ul>
        </nav>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
    *{
        /* background-color: black; */
        margin-top:-1%;
        margin-bottom: 5%;
        /* width: 100%; */
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
    .navlist{
        list-style: none;
        display: flex;
        justify-content:end; 
        position: relative;
        z-index: 100;
        width: 100%;
    }
  
</style>