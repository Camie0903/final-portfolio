<template>
    <div>
        <nav class="navheading">
            <ul class="navlist">
                <li class="navNames">
                    <router-link to="/">Home</router-link> | 
                </li> 
                <li>
                    <router-link to="/about">About</router-link> |
                </li>
                <li>
                    <router-link to="/skills">Skills</router-link> |
                </li>
                <li>
                    <router-link to="/resume">Resume</router-link> |
                </li>
                <li>
                    <router-link to="/projects">Projects</router-link> |
                </li>
                <li>
                    <router-link to="/testimonials">Testimonials</router-link> |
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
        
    }
    .navlist{
        list-style: none;
        display: flex;
        justify-content:end; 
    }
</style>