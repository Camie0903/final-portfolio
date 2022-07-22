<template>

<nav class="navbar navbar-expand-lg navbar-light ">
  <div class="container-fluid">
    <a class="navbar-brand text-white" href="#">Cameron</a>
    <button class="navbar-toggler bg-white" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon text-white"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
           <li class="navNames text-white">
                    <router-link to="/" class="nav-link mx-2 text-white">Home</router-link> 
                </li> 
                <li>
                    <router-link to="/about" class="nav-link mx-2 text-white">About</router-link>
                </li>
                <li>
                    <router-link to="/skills" class="nav-link mx-2 text-white">Skills</router-link>
                </li>
                <li>
                    <router-link to="/resume" class="nav-link mx-2 text-white">Resume</router-link> 
                </li>
                <li>
                    <router-link to="/projects" class="nav-link mx-2 text-white">Projects</router-link> 
                </li>
                <li>
                    <router-link to="/testimonials" class="nav-link mx-2 text-white">Testimonials</router-link> 
                </li>
                <li>
                    <router-link  to="/contact" class="nav-link mx-2 text-white">Contact</router-link> 
                </li>
      </ul>
    </div>
  </div>
</nav>


        <!-- <div class="container">
            <nav class="navheading">
                <a href="#" class="logo"><h2>LOGO</h2></a>
                <input type="checkbox" id="tab-nav" class="tab-nav">
                <label @click="ToggleNav" for="tab-nav" class="label">
                    <div id="burg1" class="burger"></div>
                    <div id="burg0" class="burger"></div>
                    <div id="burg2" class="burger"></div>
                </label>
                <ul class="navList" v-show="mobile">
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
        </div> -->


</template>
<script>
export default {
    data(){
        return{
            mobile:false
        }
    },
    methods: {
        ToggleNav(){
            this.mobile = true
        }
    },
}
</script>
<style scoped>
ul{
    width:100%;
    display: flex;
    justify-content: end;
}
    *{
        /* background-color: black; */
        /* margin-top:-1%;
        margin-bottom: 5%; */
        /* width: 100%; */
    }
    /* a {
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
} */
/* .container{

    width: 1280px;
    margin: auto;

} */

/* .nav_checkbox{
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    padding: 10px 0px;

} */

/* .logo{

    text-decoration: none;
    color: #fff;
    padding-left: 10px;

}

.tab-nav{
    margin:0;
    outline: none;
    display: none;

}

.label{

    display: none;
    color: #fff;

}

.burger{

    width: 35px;
    height: 5px;
    background-color: #6c6d6d;
    margin-top: 5px;
    transition:all 0.5s ease;
}

input[type=checkbox]:checked ~ .label #burg0{
  opacity:0;
}

input[type=checkbox]:checked ~ .label #burg1{
  transform: rotate(45deg) translate(7px, 7px);
  opacity: 1;
}
input[type=checkbox]:checked ~ .label #burg2{
  transform: rotate(-45deg) translate(7px, -7px);
}

.navList{

    grid-column: 3;
    list-style: none;
    margin: 0;
    padding: 0;
    
}

.navList li{

    display: inline-block;
    padding-right: 10px;

}

.navList li a{

    text-decoration: none;
    color: white;
    position: relative;

}

.navList li a::after{

    content: '';
    display: block;
    height: 2px;
    background-color: #fff;
    position: absolute;
    left: 0;
    right: 0;
    transform-origin: left;
    transform: scale(0, 1);
    transition: transform ease-in-out 0.5s;

}

.navList li a:hover::after{

    transform: scale(1, 1);

}

/* .content_section{

    height: 120vh;
    background-image: url(https://images.pexels.com/photos/4245826/pexels-photo-4245826.jpeg?cs=srgb&dl=pexels-riccardo-bertolo-4245826.jpg&fm=jpg);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    


} */

/* @media screen and (max-width: 1280px){

    .container{

        width: 100%;

    }

}

@media screen and (max-width: 770px){

    .label{

        display: grid;
        cursor: pointer;
        grid-column: 3;
        padding-right: 10px;

    }

    .navList{

        display: grid;
        grid-template-columns: 1fr;
        grid-column: 1/4;
        text-align: center;
        max-height: 0;
        overflow: hidden;
        transition: all ease-in-out 0.6s;

    }

    .nav_checkbox input:checked ~ .navList{

        max-height: 500px;

    }

    .navList li{

        padding: 15px 0px;

    }


} */
  
</style>