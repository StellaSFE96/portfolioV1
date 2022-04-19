<template>
  <section id="landing-page">
    <div class="container">
      <h1
        data-aos="fade-down"
        data-aos-delay="400"
        data-aos-easing="ease"
        data-aos-duration="2000"
      >
        <span>Hi,</span> I'm Stella.
      </h1>
      <h2
        data-aos="fade-down"
        data-aos-delay="300"
        data-aos-easing="ease"
        data-aos-duration="2000"
      >
        I'm a Frontend developer with <span> a passion for design.</span>
      </h2>
      <h3
        data-aos="fade-down"
        data-aos-delay="350"
        data-aos-easing="ease"
        data-aos-duration="2000"
      >
        I'm based in stockholm where i also study Frontend development. My aim
        is to create beautiful, accessible and human centered web experiences.
      </h3>
      <div
        class="logos"
        data-aos="fade-down"
        data-aos-delay="350"
        data-aos-easing="ease"
        data-aos-duration="2000"
      >
        <a href="https://linkedin.com/in/stella-samaranayake" target="_blank">
          <img class="linkedin-icon icon" :src="linkedin" alt="Github icon" />
        </a>
        <a href="https://github.com/StellaSFE96" target="_blank">
          <img class="git-hub-icon icon" :src="gitHub" alt="Github icon" />
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      gitHub: require("../assets/icons/gittwo.png"),
      linkedin: require("../assets/icons/linkedin.png"),
    };
  },
};
</script>

<style lang="scss" scoped>
#landing-page {
  height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  .container {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    height: 50vh;
    margin-top: 120px;
    width: 50%;

    .logos {
      margin-top: 10px;

      .git-hub-icon {
        margin-left: 15px;
        max-width: 2rem;
        transition: 300ms;
      }

      .linkedin-icon {
        max-width: 2rem;
        transition: 300ms;
      }

      .icon {
        &:hover {
          transform: translateY(-5px);
        }
      }
    }
  }

  h1 {
    font-family: "Karla", sans-serif;
    font-size: 3.8rem;
    color: #fcddec;
    span {
      color: #ce34ab;
    }
  }

  h2 {
    font-size: 2.5rem;
    max-width: 80%;
  }
  h3 {
    font-weight: 100;
  }
  h2,
  h3 {
    font-family: "Roboto", sans-serif;
    letter-spacing: 1px;
    color: #b495ad;
  }
}

@media only screen and (min-width: 370px) and (max-width: 500px) {
  #landing-page {
    height: 100vh;
    padding: 1vh;

    .container {
      width: 95%;
    }

    h1 {
      font-size: 3rem;
    }

    h2 {
      font-size: 1.3rem;
      margin-top: 20px;
    }

    h3 {
      padding-bottom: 50px;
      font-size: 1rem;
      margin-top: 20px;
    }
  }
}

@media only screen and (min-width: 500px) and (max-width: 700px) {
  #landing-page {
    height: 80vh;
    padding: 1vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .container {
      display: flex;
      flex-direction: column;
      justify-content: space-evenly;
      height: 50vh;
      margin-top: 140px;
      width: 95%;
    }

    h1 {
      font-size: 2.8rem;
    }

    h2 {
      font-size: 2rem;
      max-width: 90%;
    }
    h3 {
      font-size: 1rem;
    }
  }
}

@media only screen and (min-width: 700px) and (max-width: 900px) {
  #landing-page {
    height: 80vh;
    padding: 1vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .container {
      display: flex;
      flex-direction: column;
      justify-content: space-evenly;
      height: 50vh;
      margin-top: 120px;
      width: 80%;
    }

    h1 {
      font-size: 3rem;
    }

    h2 {
      font-size: 2.5rem;
      max-width: 90%;
    }
    h3 {
      font-size: 1.2rem;
    }
  }
}

@media only screen and (min-width: 1537px) and (max-width: 2500px) {
  #landing-page {
    height: 80vh;
    padding: 1vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .container {
      display: flex;
      flex-direction: column;
      justify-content: space-evenly;
      height: 50vh;
      margin-top: 120px;
      width: 30%;
    }
  }
}
</style>
