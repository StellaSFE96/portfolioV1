<template>
  <div id="app">
    <Header />
    <LandingPage />
    <About />
    <Experience :skills="skillsArray" />
    <Projects />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import LandingPage from "./components/LandingPage.vue";
import About from "./components/About.vue";
import Experience from "./components/Experience.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";
import skills from "./assets/data/skills.js";

export default {
  name: "App",
  components: {
    Header,
    LandingPage,
    About,
    Experience,
    Projects,
    Contact,
    Footer,
  },
  data() {
    return {
      skillsArray: [...skills],
    };
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Karla:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;1,200;1,300;1,400;1,500;1,600&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Spectral:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;1,200;1,300;1,400;1,500&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");

html {
  scroll-behavior: smooth;
}
* {
  background-color: #451149;
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}
</style>
