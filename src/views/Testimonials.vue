<template>
  <div class="he">
    <h1 class="heading" data-attr-text="Testimonials">Testimonials</h1>
  </div>
  <div class="overflow-hidden container" >
    <div class="items">
      <div class="entry" v-for="t of testimonials" :key="t.id">
        <p class="name">{{t.name}}</p>
        <img :src="t.imgUrl" />
        <p class="quote">"{{t.testi}}"</p>
      </div>
    </div>
    <!-- <div class="controls">
      <button class="prev" @click="prevTestimonial">&#8249;</button>
      <button class="next" @click="nextTestimonial">&#8250;</button>
    </div> -->
  </div>
</template>
<script>
export default {
    data(){
      return {
        testimonials: [
        {
            id: 1,
            imgUrl:"https://i.postimg.cc/brWdqkyH/Chanique-2.jpg",
            name: "Chanique Mansoor",
            testi:"Cameron is a dedicated and determined women who loves being social, she strives in her work and is always willing to help."
        },
        {
            id: 2,
            imgUrl:"https://i.postimg.cc/d1J59TKB/jason.jpg",
            name: "Jason Wandrag",
            testi:"Cameron has shown great potential with her work in web development. She strives to do her best and I am certain that she will continue to learn and grow as a software developer."
        },
        {
            id: 3,
            imgUrl:"https://i.postimg.cc/YqLJXVPy/Sunethia-1.jpg",
            name: "Sunethia Lawrence",
            testi:"Cameron is a loyal, hardworking and commited young lady, who takes her work serious and makes sure she achieve her goals. It's always a pleasure working because of the positive vibe she has."
        },
        {
            id: 4,
            imgUrl:"https://i.postimg.cc/qRVvDyJ9/Hilmi-1.jpg",
            name: "Hilmi Mallick",
            testi:"Cameron is a very hardworking and disciplined young women who always strives to improve herself and those around her."
        } ,
        {
            id: 5,
            imgUrl:"https://i.postimg.cc/XqmGQN8s/IMG-20220721-WA0010.jpg",
            name: "Yaaseen Davids",
            testi:"Cameron is consistent, dependable and accurate in carrying out responsibilities to a successful conclusion. She also display an ability to learn rapidly and adapt quickly to changing situations."
        },
        {
            id: 6,
            imgUrl:"https://i.postimg.cc/XqjVKwW4/Siyolise-1.jpg",
            name: "Siyolise Mekuto",
            testi:"Cameron is a delightful person to work with. She is always proving herself when it comes to coding and very reliable."
        },
        {
            id: 7,
            imgUrl:"https://i.postimg.cc/1R8HrbWn/homepic.jpg",
            name: "Jesse Spence",
            testi:"Cameron is a reliable work colleague to have, you can always count on her to complete what is needed. This along with her great energy and easy going personality makes her an absolute asset to have in any work environment."
        },
        // {
        //     id: 8,
        //     imgUrl:"https://i.postimg.cc/qRVvDyJ9/Hilmi-1.jpg",
        //     name: "Hilmi Mallick",
        //     testi:"Cameron is a very hardworking and disciplined young women who always strives to improve herself and those around her."
        // } ,
        ],
      currentTestimonialIndex: 0
    };
  },
  methods: {
    prevTestimonial() {
      this.currentTestimonialIndex =
        (this.currentTestimonialIndex - 1 + this.testimonials.length) %
        this.testimonials.length;
    },
    nextTestimonial() {
      this.currentTestimonialIndex =
        (this.currentTestimonialIndex + 1) % this.testimonials.length;
    }
  }
};

</script>
<style scoped>
/* body{
  overflow: hidden;
} */
/* .container {
    position: relative;
    
  } */

  .items {
    display: flex;
    align-items: center;
    width: fit-content;
    overflow:visible;
    animation: carouselAnim 80s infinite alternate linear;
  }

  .controls {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    display: flex;
    justify-content: space-between;
    width: 100%;
    padding: 0 20px;
    box-sizing: border-box;
  }

  .prev,
  .next {
    border: none;
    background: none;
    font-size: 2em;
    color: #666;
    cursor: pointer;
  }

  @media screen and (max-width: 768px) {
    .items {
      animation: none;
    }
  }
h1 {
  letter-spacing: 1.5px;
  color: white;
  font-weight: 400;
  color: white;
  font-family: "Righteous", serif;
  font-size: 4.4rem;
  text-shadow: 0.03em 0.03em 0 hsla(230, 40%, 50%, 1);
  text-align: center;

  margin-top: -10%;
  position: relative;
}
.he{
 margin-top: 20vh;
 }

img {
  width: 50%;
  border-radius: 50%;
  height: 140px;
}

.container {
  width: 100%;
  overflow: hidden;
  position: relative;
}

.items {
  display: flex;
  align-items: center;
  width: fit-content;
  animation: carouselAnim 80s infinite alternate linear;
}

.entry {
  display: flex;
  align-items: center;
  flex-direction: column;
  position: relative;
  width: 300px;
  background: #fff;
  margin: 1em;
  padding: 0.5em;
  border-radius: 10px;
  box-shadow: 4px 4px 5px 0px rgba(0, 0, 0, 0.5);
  color: #222;
}

@media only screen and (max-width: 768px) {
  .items {
    animation: carouselAnim 100s infinite alternate linear;
  }
  
  @keyframes carouselAnim {
    from {
      transform: translate(0, 0);
    }
    to {
      transform: translate(calc(-100% + (2 * 300px)));
    }
  }
}
@media screen and (max-width: 750px) {
  .items {
    /* animation: none; */
    animation: carouselAnim2 100s infinite alternate linear;
    flex-direction: column;
    display: flex;
    justify-content: center;
    padding-left: 2rem;
    padding-right: 0;
  }
  @keyframes carouselAnim2 {
    from {
      transform: translatey(0);
    }
    to {
      transform: translatey( calc(-100% + (2 * 300px)));
    }
  }
}
.entry p {
  text-align: center;
  padding: 1em;
}

.name {
  font-weight: bold;
}

@keyframes carouselAnim {
  from {
    transform: translate(0, 0);
  }
  to {
    transform: translate(calc(-100% + (5 * 300px)));
  }
}

.container .faders {
  width: 100%;
  height: 100%;
}

.faders .right,
.faders .left {
  background: linear-gradient(
    to right,
    rgba(245, 245, 245, 1) 0%,
    rgba(255, 255, 255, 0) 100%
  );
  width: 15%;
  height: 100%;
  position: absolute;
  z-index: 200;
}

.right {
  right: 0;
  background: linear-gradient(
    to left,
    rgba(245, 245, 245, 1) 0%,
    rgba(255, 255, 255, 0) 100%
  );
}
/* Add this media query for screens with a maximum width of 768px (tablet size) */
@media screen and (max-width: 768px) {
  /* Move the carousel up */
  .carousel {
    transform: translateY(-50%);
    top: 50%;
  }
  
  /* Adjust the width of the carousel item */
  .carousel-item {
    width: 100%;
  }
  
  /* Hide the carousel controls */
  .carousel-control-prev,
  .carousel-control-next {
    display: none;
  }
}

/* Add this media query for screens with a maximum width of 576px (mobile size) */
@media screen and (max-width: 576px) {
  /* Move the carousel up further */
  .carousel {
    transform: translateY(-75%);
    top: 50%;
  }
}


</style>