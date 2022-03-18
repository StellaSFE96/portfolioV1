<template>
  <div id="header">
    <div class="container">
      <div class="logo-container">
        <h1
          class="logo"
          data-aos="fade-down"
          data-aos-delay="1000"
          data-aos-easing="ease"
          data-aos-duration="2000"
        >
          SS
        </h1>
      </div>
      <div class="nav-container">
        <a
          class="link link-1"
          href="#about"
          data-aos="fade-down"
          data-aos-delay="900"
          data-aos-easing="ease"
          data-aos-duration="2000"
          >ABOUT</a
        >
        <a
          class="link link-2"
          href="#experience"
          data-aos="fade-down"
          data-aos-delay="800"
          data-aos-easing="ease"
          data-aos-duration="2000"
        >
          EXPERIENCE</a
        >
        <a
          class="link link-3"
          href="#projects"
          data-aos="fade-down"
          data-aos-delay="700"
          data-aos-easing="ease"
          data-aos-duration="2000"
          >WORK</a
        >
        <a
          class="link link-4"
          href="#contact"
          data-aos="fade-down"
          data-aos-delay="600"
          data-aos-easing="ease"
          data-aos-duration="2000"
          >CONTACT</a
        >
        <a
          class="resume link link-5"
          href=""
          data-aos="fade-down"
          data-aos-delay="500"
          data-aos-easing="ease"
          data-aos-duration="2000"
          >RESUME</a
        >
      </div>
    </div>
  </div>
</template>

<script></script>

<style lang="scss" scoped>
#header {
  width: 100%;
  height: 100px;
  background-color: #451149;
  position: fixed;
}
.container {
  display: flex;
  padding-top: 30px;
}

.logo-container {
  width: 50%;
  h1 {
    margin-left: 30px;
    color: #ce34ab;
    font-family: "Karla", sans-serif;
    font-size: 2.5rem;
  }
}

.nav-container {
  width: 50%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  padding-left: 100px;

  .link {
    color: #b495ad;
    font-family: "Karla", sans-serif;
    font-size: 1rem;
    text-decoration: none;
    transition: 50ms;

    &:hover {
      color: #ce34ab;
    }
  }

  .link-5 {
    color: #ce34ab;
  }

  .resume {
    border: 1px solid rgb(137, 53, 139);
    border-radius: 6px;
    padding: 7px;
    box-shadow: 1px 1px 1px rgb(207, 85, 177);

    &:hover {
      background-color: #5a165f;
    }
  }
}
</style>
