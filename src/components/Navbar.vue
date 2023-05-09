<!-- <template>
    <nav class="navbar navbar-expand-lg navbar-light ">
      <div class="container-fluid">
        <a class="navbar-brand text-white" href="/">Cameron</a>
        <button
          class="navbar-toggler bg-white"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon text-white"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link to="/" class="nav-link text-white">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link text-white">About</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/skills" class="nav-link text-white">Skills</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/resume" class="nav-link text-white">Resume</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/projects" class="nav-link text-white">Projects</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/testimonials" class="nav-link text-white">Testimonials</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/contact" class="nav-link text-white">Contact</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </template>
  
  <style scoped>
    .navbar-nav {
      margin-left: auto;
    }
    .nav-item {
      margin-right: 10px;
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
  </style>

   -->
<template>
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

<style>
/* Style the side navbar */
.sidenav {
  height: 100%;
  width: 200px;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: #000;
  overflow-x: hidden;
  padding-top: 20px;
}

/* Add styles to the links in the side navbar */
.sidenav a {
  padding: 6px 8px 6px 16px;
  text-decoration: none;
  font-size: 20px;
  color: #818181;
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

</style>