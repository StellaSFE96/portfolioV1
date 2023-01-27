<template>
  <section id="about">
    <div
      class="container"
      data-aos="fade-right"
      data-aos-duration="1600"
      data-aos-easing="ease"
      data-aos-once="false"
      data-aos-delay="200"
    >
      <h1>/ About me</h1>
      <p>
        I'm currently <strong>studying</strong> Frontend development at the
        <strong>IT College</strong> in Stockholm. I have great interest in
        Design, Technology and everything in between. Follow me on my
        <strong>journey</strong> to learn coding.
      </p>
      <p>
        Now I'm looking for my second Frontend Developer
        <strong>internship</strong> where I get to use my
        <strong>curiosity</strong>, <strong>drive</strong> and prior
        <strong>experience</strong>
        in retail and customer service to contribute to future projects and to
        <strong>grow</strong> as a developer.
      </p>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#about {
  height: 95vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  .container {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    height: 50vh;
    width: 50%;

    h1 {
      font-family: "Karla", sans-serif;
      font-size: 3rem;
      color: #ce34ab;
    }

    p {
      font-family: "Roboto", sans-serif;
      font-size: 1.1rem;
      letter-spacing: 1px;
      color: #b495ad;
    }

    strong {
      color: #fcddec;
      transition: 400ms ease-out;

      &:hover {
        color: #ce34ab;
      }
    }
  }
}

@media only screen and (min-width: 370px) and (max-width: 760px) {
  #about {
    height: 100vh;
    padding: 1vh;

    .container {
      width: 95%;

      h1 {
        font-size: 3rem;
      }

      p {
        font-size: 1rem;
        margin-top: 20px;
      }

      p:nth-of-type(2) {
        margin-top: 20px;
      }
    }
  }
}

@media only screen and (min-width: 1537px) and (max-width: 2560px) {
  #about {
    height: 100vh;
    padding: 1vh;

    .container {
      width: 30%;

      h1 {
        font-size: 3rem;
      }

      p {
        font-size: 1rem;
        margin-top: 20px;
      }

      p:nth-of-type(2) {
        margin-top: 20px;
      }
    }
  }
}
</style>
