<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container-fluid">
      <a class="navbar-brand text-white" href="/">Cameron</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
        @click="isNavOpen = !isNavOpen"
      >
        <span class=""><i class="fa-solid fa-bars-staggered" style="color: #ffffff;"></i></span>
      </button>
      <div class="collapse navbar-collapse" :class="{ show: isNavOpen }" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link to="/" class="nav-link text-white" @click="isNavOpen = false">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/about" class="nav-link text-white" @click="isNavOpen = false">About</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/skills" class="nav-link text-white" @click="isNavOpen = false">Skills</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/resume" class="nav-link text-white" @click="isNavOpen = false">Resume</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/projects" class="nav-link text-white" @click="isNavOpen = false">Projects</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/testimonials" class="nav-link text-white" @click="isNavOpen = false">Testimonials</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/contact" class="nav-link text-white" @click="isNavOpen = false">Contact</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isNavOpen: false,
    };
  },
};
</script>

  
  <style scoped>
  
  .navbar{
    z-index: 1;
  }
    .navbar-nav {
      margin-left: auto;
    }
    .nav-item {
      margin-right: 10px;
    
  color:white;
  font-family: 'Merienda', cursive;
  animation-name:glow;
  animation-duration:1s;
  animation-iteration-count:infinite;
  animation-direction:alternate;
}
@keyframes glow {
  from {
    text-shadow: 0px 0px 5px #c9d9ff, 0px 0px 5px #2a3e92;
  }
  to {
    text-shadow: 0px 0px 20px #c9d9ff, 0px 0px 20px #2a3e92;
  }
}

    
    @media (max-width: 991.98px) {
      .nav-item {
        margin-right: 5px;
      }
    }
    @media (max-width: 767.98px) {
      .nav-link {
        padding: 0.5rem 0 !important;
      }
    }
    @media only screen and (max-width: 991.98px) {
  .navbar {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: rgb(0 0 0 / 80%);
    z-index: 9999;
  }
}

  </style>



<!-- <template>
    <div class="sidenav">
    <a href="/">Home</a>
    <a href="/about">About</a>
    <a href="/skills">Skills</a>
    <a href="/projects">Projects</a>
    <a href="/resume">Resume</a>
    <a href="/testimonials">Testimonials</a>
    <a href="/contact">Contact</a>
  </div>
  

  
</template>

<style> -->
<!-- /* Style the side navbar */ -->
<!-- .sidenav {
  height: 100%;
  width: 200px;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: #000;
  overflow-x: hidden;
  padding-top: 20px;
} -->

<!-- /* Add styles to the links in the side navbar */
.sidenav a {
  padding: 6px 8px 6px 16px;
  text-decoration: none;
  font-size: 20px;
  color: #fff;
  display: block;
}

/* Change the color of links on hover */
.sidenav a:hover {
  color: #f1f1f1;
}

/* Style the main content */
.main {
  margin-left: 200px; /* Same as the width of the sidenav */
  padding: 0px 10px;
}

/* Add media query for smaller screens */
@media screen and (max-height: 450px) {
  .sidenav {padding-top: 15px;}
  .sidenav a {font-size: 18px;}
}
/* Add media query for smaller screens */
@media screen and (min-height: 1008px) {
  .sidenav {
    display: flex;
    flex-direction: row;
    padding-top: 15px;
    position: absolute;
    top: 0;
    background-color: initial;
  }
  .sidenav a {
    display: flex;
    flex-direction: row;
    font-size: 18px;
  }
}

/* Add media query for even smaller screens */
@media screen and (min-width: 490px) {
  .sidenav {
    position: absolute;
    top: 0;
  }
}


</style> -->

