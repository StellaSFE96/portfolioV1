<template>
  <section id="contact">
    <div class="container">
      <vue-typed-js
        :showCursor="false"
        :strings="['...']"
        :startDelay="1000"
        :typeSpeed="1000"
        :loop="true"
        ><h1>/ Get in touch<span class="typing"></span></h1
      ></vue-typed-js>
      <p>
        As I am currently looking for a new opportunity I would love to hear
        from you! My inbox is always open whether you have a question or just
        want to connect, feel free to reach out.
      </p>
      <a
        class="button"
        href="mailto: stella.samaranayake@outlook.com?subject=Let's connect!"
        target="_blank"
      >
        Say Hello
      </a>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#contact {
  height: 60vh;
  padding-bottom: 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  .container {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: center;
    width: 40%;
    height: 60%;
    text-align: center;

    h1 {
      font-family: "Karla", sans-serif;
      font-size: 3rem;
      color: #ce34ab;
      margin-bottom: 20px;
    }

    p {
      font-family: "Roboto", sans-serif;
      font-size: 1rem;
      letter-spacing: 1px;
      color: #b495ad;
    }

    .button {
      height: 3rem;
      width: 11rem;
      font-family: "Karla", sans-serif;
      text-decoration: none;
      border: none;
      background-color: #bb349b;
      border-radius: 30px;
      color: #f1c1e6;
      font-size: 1.5em;
      margin-top: 2rem;
      padding: 6px;
      transition: transform 300ms ease-in-out;

      &:hover {
        background-color: #ad3090;
        transform: scale(1.1);
      }
    }

    span {
      margin-left: 10px;
    }
  }
}

@media only screen and (min-width: 370px) and (max-width: 500px) {
  #contact {
    // padding: 2vh;
    padding: 40vh 1vh;

    .container {
      width: 100%;

      h1 {
        font-size: 2.2rem;
      }
    }
  }
}

@media only screen and (min-width: 500px) and (max-width: 1115px) {
  #contact {
    padding: 40vh 1vh;

    .container {
      width: 85%;

      h1 {
        font-size: 3rem;
      }

      p {
        margin-top: 20px;
      }
    }
  }
}

@media only screen and (min-width: 1537px) and (max-width: 2560px) {
  #contact {
    padding: 40vh 1vh;

    .container {
      width: 32%;

      p {
        margin-top: 40px;
      }

      .button {
        margin-top: 100px;
      }
    }
  }
}
</style>
