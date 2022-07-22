<template>
<div class="he">
  <h1>Testimonials</h1>
</div>
  <div class="items">
    <div class="entry" v-for="t of testimonials" :key="t.id">
      <p class="name">{{t.name}}</p>
      <img :src="t.imgUrl" />
      <p class="quote">"{{t.testi}}"</p>
    </div>
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
        {
            id: 8,
            imgUrl:"https://i.postimg.cc/qRVvDyJ9/Hilmi-1.jpg",
            name: "Hilmi Mallick",
            testi:"Cameron is a very hardworking and disciplined young women who always strives to improve herself and those around her."
        } ,
]
      }
    }
}

</script>
<style scoped>
.he{
  margin-top: -13%;
  position: relative;
  z-index: 100;
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
    h1 {
  text-align: center;
  margin: 1.5em;
  margin-top: -10%;
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
@media screen and (max-width: 400px) {
  .items {
    /* animation: none; */
    animation: carouselAnim2 100s infinite alternate linear;
    flex-direction: column;
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
  position: absolute;
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

</style>