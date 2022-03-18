<template>
  <div id="header">
    <div class="container">
      <div class="logo-container">
        <h1 class="logo">SS</h1>
      </div>
      <div class="nav-container">
        <a class="link link-1" href="#about">ABOUT</a>
        <a class="link link-2" href="#experience">EXPERIENCE</a>
        <a class="link link-3" href="#projects">WORK</a>
        <a class="link link-4" href="#contact">CONTACT</a>
        <a class="resume link link-5" href="">RESUME</a>
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
