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
        data-aos-delay="300"
        data-aos-easing="ease"
        data-aos-duration="2000"
      >
        I'm based in stockholm where i also study Frontend development.
        <span
          >My aim is to create beautiful, accessible and human centered web
          experiences.
        </span>
      </h3>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#landing-page {
  height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  padding-left: 30vh;

  .container {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    height: 50vh;
    margin-top: 120px;
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
  }
  h3 {
    font-weight: 100;
  }
  h2,
  h3 {
    font-family: "Roboto", sans-serif;
    letter-spacing: 1px;
    color: #b495ad;

    span {
      display: block;
    }
  }
}
</style>
