<template>
  
  
  <div id="container">
    <div class="background-container">
<img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/1231630/moon2.png" alt="">
<div class="stars"></div>
<div class="twinkling"></div>
<div class="clouds"></div>
</div>
    <div id="content">
      <div id="about">
        <h1>
          <div class="heading1" style="float:initial; margin-top:14rem; color: #fff;">
            <span ref="text1Container"></span>
            <span ref="textContainer"></span>
          </div>
        </h1>
      </div>
    </div>
  </div>
</template>

<style scoped>

  /* desktop styles */
  .container {
    width: 100%;
    max-width: 960px;
    margin: 0 auto;
  }
  .box {
    background-color: #f1f1f1;
    padding: 20px;
    border: 1px solid #ccc;
  }

  /* tablet styles */
  @media (max-width: 768px) {
    .container {
      max-width: 768px;
    }
    .box {
      padding: 15px;
    }
  }

  /* cellphone styles */
  @media (max-width: 480px) {
    .container {
      max-width: 480px;
    }
    .box {
      padding: 10px;
    }
    .heading1{
      padding-top: 12rem;
      font-size: 2rem;
    }
  }

#content{
  position: relative;
  z-index: 4;
}
.heading1 {
  z-index: 1;
  margin-top: 14rem; 
  color: #fff;
  font-size: 3rem;
  background-color: rgba(0, 0, 0, 0.5); /* black with 50% opacity */
  display: inline-block; /* set display to inline-block */
}
@keyframes move-background {
  from {
    -webkit-transform: translate3d(0px, 0px, 0px);
  }
  to {
    -webkit-transform: translate3d(1000px, 0px, 0px);
  }
}
@-webkit-keyframes move-background {
  from {
    -webkit-transform: translate3d(0px, 0px, 0px);
  }
  to {
    -webkit-transform: translate3d(1000px, 0px, 0px);
  }
}
@-moz-keyframes move-background {
  from {
    -webkit-transform: translate3d(0px, 0px, 0px);
  }
  to {
    -webkit-transform: translate3d(1000px, 0px, 0px);
  }
}
@-webkit-keyframes move-background {
  from {
    -webkit-transform: translate3d(0px, 0px, 0px);
  }
  to {
    -webkit-transform: translate3d(1000px, 0px, 0px);
  }
}
.background-container {
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

.stars {
  background: black url(https://s3-us-west-2.amazonaws.com/s.cdpn.io/1231630/stars.png) repeat;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  display: block;
  z-index: 0;
}

.twinkling {
  width: 10000px;
  height: 100%;
  background: transparent url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/1231630/twinkling.png") repeat;
  background-size: 1000px 1000px;
  position: absolute;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: 2;
  -moz-animation: move-background 70s linear infinite;
  -ms-animation: move-background 70s linear infinite;
  -o-animation: move-background 70s linear infinite;
  -webkit-animation: move-background 70s linear infinite;
  animation: move-background 70s linear infinite;
}

.clouds {
  width: 10000px;
  height: 100%;
  background: transparent url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/1231630/clouds_repeat.png") repeat;
  background-size: 1000px 1000px;
  position: absolute;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: 3;
  -moz-animation: move-background 150s linear infinite;
  -ms-animation: move-background 150s linear infinite;
  -o-animation: move-background 150s linear infinite;
  -webkit-animation: move-background 150s linear infinite;
  animation: move-background 150s linear infinite;
}

img {
  height: 70vh;
  width: 70vh;
  position: absolute;
  z-index: 3;
  right: 20px;
}

body {
  background-color: #000;
  /* background-image:url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0naHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmcnIHdpZHRoPScxMDAlJyBoZWlnaHQ9JzEyMCc+Cgk8ZGVmcz4KCQk8cGF0dGVybiBwYXR0ZXJuVW5pdHM9J3VzZXJTcGFjZU9uVXNlJyBpZD0nYycgd2lkdGg9JzYwJyBoZWlnaHQ9JzEyMCcgeD0nMCcgeT0nMCcgdmlld0JveD0nMCAwIDUgMTAnPgoJCQk8cGF0aCBmaWxsLW9wYWNpdHk9JzAnIHN0cm9rZT0nIzI5MjkyOScgc3Ryb2tlLXdpZHRoPScwLjA5JyBkPSdNLTIsMUw3LDEwTS0yLDZMNywxNU0tMiwtNEw3LDUnLz4KCQk8L3BhdHRlcm4+CgkJPHBhdHRlcm4gcGF0dGVyblVuaXRzPSd1c2VyU3BhY2VPblVzZScgaWQ9J2MyJyB3aWR0aD0nNjAnIGhlaWdodD0nMTIwJyB4PScxMDAlJyB5PScwJyB2aWV3Qm94PScwIDAgNSAxMCc+CgkJCTxwYXRoIGZpbGwtb3BhY2l0eT0nMCcgc3Ryb2tlPScjMjkyOTI5JyBzdHJva2Utd2lkdGg9JzAuMDknIGQ9J003LDFMLTIsMTBNNyw2TC0yLDE1TTcsLTRMLTIsNScvPgoJCTwvcGF0dGVybj4KCTwvZGVmcz4KCTxyZWN0IHdpZHRoPSc1MCUnIGhlaWdodD0nMTAwJScgZmlsbD0ndXJsKCNjKScvPgoJPHJlY3QgeD0nNTAlJyB3aWR0aD0nNTAlJyBoZWlnaHQ9JzEwMCUnIGZpbGw9J3VybCgjYzIpJy8+Cjwvc3ZnPg=='); */
  background-image:url('https://i.postimg.cc/0Nx8DvrV/Untitled-design-1.png');
   width: 100vw;
    margin:0; padding:0;
    overflow-x:hidden;
    height:100%;
    font-family: 'Lato', Helvetica, arial, sans-serif;
    font-weight: 300;
    font-size: 20px;
    line-height: 1.45;
    color: #eee;
    color: rgba(255,255,255,.85);
}
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.typing {
  display: inline-block;
  font-size: 2rem;
  font-weight: bold;
  color: #fff;
  overflow: hidden;
  white-space: nowrap;
  border-right: 0.1em solid #fff;
  animation: typing 3s steps(40) infinite;
}

@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

.word {
  display: inline-block;
  padding-right: 0.5em;
}
</style>

<script>
    export default {
  data() {
    return {
      text1: [
        "Hi :)",
      ],
      text: [
        "My name is Cameron Tamboer",
        "I'm an enthusiastic web developer,",
        "with a strong passion for creating, ", 
        "maintaining responsive websites.",
      ],
    };
  },
  methods: {
    waitForMs(ms) {
      return new Promise((resolve) => setTimeout(resolve, ms));
    },
    async typeSentence(sentence, containerRef, delay = 70) {
      let letters = sentence.split("");
      let i = 0;
      while (i < letters.length) {
        await this.waitForMs(delay);
        containerRef.append(letters[i]);
        i++;
      }
    },
    async deleteSentence(containerRef) {
      let sentence = containerRef.innerHTML;
      let letters = sentence.split("");
      while (letters.length > 0) {
        await this.waitForMs(80);
        letters.pop();
        containerRef.innerHTML = letters.join("");
      }
    },
    async sentenceLoop(sentenceList1, sentenceList2) {
      let i = 0;
      let isSecondListDone = false;
      while (true) {
        await this.typeSentence(sentenceList1[i], this.$refs.textContainer);
        await this.waitForMs(800); // Pause after sentence is typed
        await this.deleteSentence(this.$refs.textContainer);
        await this.waitForMs(200); // Pause after sentence is deleted
        i++;
        if (i >= sentenceList1.length) {
          i = 0;
          sentenceList1 = sentenceList2;
          isSecondListDone = true;
        }
        if (isSecondListDone && i >= sentenceList2.length) {
          // Add clickable word after the text array
          this.$refs.textContainer.innerHTML += '<span class="clickable-word">Click me</span>';
          const clickableWord = this.$refs.textContainer.querySelector('.clickable-word');
          clickableWord.addEventListener('click', this.handleClick);
          break;
        }
      }
    },
    handleClick() {
      // Handle click on the clickable word
      console.log('Clicked!');
    },
  },
  async mounted() {
    await this.sentenceLoop(this.text1, this.text);
  },
}

</script>