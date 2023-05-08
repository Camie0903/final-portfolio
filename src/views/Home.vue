<template>
  <div id="container">
    <div id="content">
      <div id="about">
        <h1>
          <div class="heading1" style='float:initial; margin-top:14rem; color: #fff;'>
            <h2><span ref="text1Container"></span></h2>
            <h2><span ref="textContainer"></span></h2>
          </div>
        </h1>
      </div>
    </div>
  </div>
</template>

<style>
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
        "and I'm an enthusiastic web developer",
        "with a strong passion for creating engaging and responsive websites.",
      ],
    };
  },
  methods: {
    waitForMs(ms) {
      return new Promise((resolve) => setTimeout(resolve, ms));
    },
    async typeSentence(sentence, containerRef, delay = 100) {
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
        await this.waitForMs(100);
        letters.pop();
        containerRef.innerHTML = letters.join("");
      }
    },
    async sentenceLoop(sentenceList1, sentenceList2) {
      let i = 0;
      let isSecondListDone = false;
      while (true) {
        await this.typeSentence(sentenceList1[i], this.$refs.textContainer);
        await this.waitForMs(1500); // Pause after sentence is typed
        await this.deleteSentence(this.$refs.textContainer);
        await this.waitForMs(500); // Pause after sentence is deleted
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
