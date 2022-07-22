<template>
 <Navbar/>
  <router-view/>
  <Footer />
</template>
<script>
import Navbar from "./components/Navbar.vue";
import Footer from ".footer.vue";
export default {
  name: "App",
  components: {
    Navbar,
    Footer,
  }
};
</script>

<style>
@font-face {
  font-family: 'Chivo';
  font-style: italic;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/chivo/v17/va9D4kzIxd1KFrBteUp9gK_uQQ.ttf) format('truetype');
}
@font-face {
  font-family: 'Chivo';
  font-style: italic;
  font-weight: 400;
  src: url(https://fonts.gstatic.com/s/chivo/v17/va9G4kzIxd1KFrBtceFfkA.ttf) format('truetype');
}
@font-face {
  font-family: 'Chivo';
  font-style: italic;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/chivo/v17/va9D4kzIxd1KFrBteVp6gK_uQQ.ttf) format('truetype');
}
@font-face {
  font-family: 'Chivo';
  font-style: italic;
  font-weight: 900;
  src: url(https://fonts.gstatic.com/s/chivo/v17/va9D4kzIxd1KFrBteWJ4gK_uQQ.ttf) format('truetype');
}
@font-face {
  font-family: 'Chivo';
  font-style: normal;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/chivo/v17/va9F4kzIxd1KFrjDY_Z4sKg.ttf) format('truetype');
}
@font-face {
  font-family: 'Chivo';
  font-style: normal;
  font-weight: 400;
  src: url(https://fonts.gstatic.com/s/chivo/v17/va9I4kzIxd1KFrBoQeY.ttf) format('truetype');
}
@font-face {
  font-family: 'Chivo';
  font-style: normal;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/chivo/v17/va9F4kzIxd1KFrjTZPZ4sKg.ttf) format('truetype');
}
@font-face {
  font-family: 'Chivo';
  font-style: normal;
  font-weight: 900;
  src: url(https://fonts.gstatic.com/s/chivo/v17/va9F4kzIxd1KFrjrZvZ4sKg.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira';
  font-style: normal;
  font-weight: 100;
  font-stretch: normal;
  src: url(https://fonts.gstatic.com/s/saira/v14/memWYa2wxmKQyPMrZX79wwYZQMhsyuShhKMjjbU9uXuA71rDks8xkw.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira';
  font-style: normal;
  font-weight: 200;
  font-stretch: normal;
  src: url(https://fonts.gstatic.com/s/saira/v14/memWYa2wxmKQyPMrZX79wwYZQMhsyuShhKMjjbU9uXuA79rCks8xkw.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira';
  font-style: normal;
  font-weight: 300;
  font-stretch: normal;
  src: url(https://fonts.gstatic.com/s/saira/v14/memWYa2wxmKQyPMrZX79wwYZQMhsyuShhKMjjbU9uXuA7wTCks8xkw.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira';
  font-style: normal;
  font-weight: 400;
  font-stretch: normal;
  src: url(https://fonts.gstatic.com/s/saira/v14/memWYa2wxmKQyPMrZX79wwYZQMhsyuShhKMjjbU9uXuA71rCks8xkw.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira';
  font-style: normal;
  font-weight: 500;
  font-stretch: normal;
  src: url(https://fonts.gstatic.com/s/saira/v14/memWYa2wxmKQyPMrZX79wwYZQMhsyuShhKMjjbU9uXuA72jCks8xkw.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira';
  font-style: normal;
  font-weight: 600;
  font-stretch: normal;
  src: url(https://fonts.gstatic.com/s/saira/v14/memWYa2wxmKQyPMrZX79wwYZQMhsyuShhKMjjbU9uXuA74TFks8xkw.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira';
  font-style: normal;
  font-weight: 700;
  font-stretch: normal;
  src: url(https://fonts.gstatic.com/s/saira/v14/memWYa2wxmKQyPMrZX79wwYZQMhsyuShhKMjjbU9uXuA773Fks8xkw.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira';
  font-style: normal;
  font-weight: 800;
  font-stretch: normal;
  src: url(https://fonts.gstatic.com/s/saira/v14/memWYa2wxmKQyPMrZX79wwYZQMhsyuShhKMjjbU9uXuA79rFks8xkw.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira Extra Condensed';
  font-style: normal;
  font-weight: 100;
  src: url(https://fonts.gstatic.com/s/sairaextracondensed/v11/-nFsOHYr-vcC7h8MklGBkrvmUG9rbpkisrTri3j2_Co.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira Extra Condensed';
  font-style: normal;
  font-weight: 200;
  src: url(https://fonts.gstatic.com/s/sairaextracondensed/v11/-nFvOHYr-vcC7h8MklGBkrvmUG9rbpkisrTrJ2nh2wpk.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira Extra Condensed';
  font-style: normal;
  font-weight: 300;
  src: url(https://fonts.gstatic.com/s/sairaextracondensed/v11/-nFvOHYr-vcC7h8MklGBkrvmUG9rbpkisrTrQ2rh2wpk.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira Extra Condensed';
  font-style: normal;
  font-weight: 400;
  src: url(https://fonts.gstatic.com/s/sairaextracondensed/v11/-nFiOHYr-vcC7h8MklGBkrvmUG9rbpkisrTj6Ejx.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira Extra Condensed';
  font-style: normal;
  font-weight: 500;
  src: url(https://fonts.gstatic.com/s/sairaextracondensed/v11/-nFvOHYr-vcC7h8MklGBkrvmUG9rbpkisrTrG2vh2wpk.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira Extra Condensed';
  font-style: normal;
  font-weight: 600;
  src: url(https://fonts.gstatic.com/s/sairaextracondensed/v11/-nFvOHYr-vcC7h8MklGBkrvmUG9rbpkisrTrN2zh2wpk.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira Extra Condensed';
  font-style: normal;
  font-weight: 700;
  src: url(https://fonts.gstatic.com/s/sairaextracondensed/v11/-nFvOHYr-vcC7h8MklGBkrvmUG9rbpkisrTrU23h2wpk.ttf) format('truetype');
}
@font-face {
  font-family: 'Saira Extra Condensed';
  font-style: normal;
  font-weight: 800;
  src: url(https://fonts.gstatic.com/s/sairaextracondensed/v11/-nFvOHYr-vcC7h8MklGBkrvmUG9rbpkisrTrT27h2wpk.ttf) format('truetype');
}
h1 {
  font-family: 'Saira', sans-serif;
  letter-spacing: 1.5px;
  color: white;
  font-weight: 400;
  font-size: 2.4em;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  
}
body {
  background-color: #141414;
  background-image:url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0naHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmcnIHdpZHRoPScxMDAlJyBoZWlnaHQ9JzEyMCc+Cgk8ZGVmcz4KCQk8cGF0dGVybiBwYXR0ZXJuVW5pdHM9J3VzZXJTcGFjZU9uVXNlJyBpZD0nYycgd2lkdGg9JzYwJyBoZWlnaHQ9JzEyMCcgeD0nMCcgeT0nMCcgdmlld0JveD0nMCAwIDUgMTAnPgoJCQk8cGF0aCBmaWxsLW9wYWNpdHk9JzAnIHN0cm9rZT0nIzI5MjkyOScgc3Ryb2tlLXdpZHRoPScwLjA5JyBkPSdNLTIsMUw3LDEwTS0yLDZMNywxNU0tMiwtNEw3LDUnLz4KCQk8L3BhdHRlcm4+CgkJPHBhdHRlcm4gcGF0dGVyblVuaXRzPSd1c2VyU3BhY2VPblVzZScgaWQ9J2MyJyB3aWR0aD0nNjAnIGhlaWdodD0nMTIwJyB4PScxMDAlJyB5PScwJyB2aWV3Qm94PScwIDAgNSAxMCc+CgkJCTxwYXRoIGZpbGwtb3BhY2l0eT0nMCcgc3Ryb2tlPScjMjkyOTI5JyBzdHJva2Utd2lkdGg9JzAuMDknIGQ9J003LDFMLTIsMTBNNyw2TC0yLDE1TTcsLTRMLTIsNScvPgoJCTwvcGF0dGVybj4KCTwvZGVmcz4KCTxyZWN0IHdpZHRoPSc1MCUnIGhlaWdodD0nMTAwJScgZmlsbD0ndXJsKCNjKScvPgoJPHJlY3QgeD0nNTAlJyB3aWR0aD0nNTAlJyBoZWlnaHQ9JzEwMCUnIGZpbGw9J3VybCgjYzIpJy8+Cjwvc3ZnPg==');
  
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

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
