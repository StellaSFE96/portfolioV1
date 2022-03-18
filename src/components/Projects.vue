<template>
  <section id="projects">
    <div class="container">
      <h1>/ Projects</h1>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#projects {
  background-color: #451149;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  padding-left: 30vh;

  .container {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    height: 30vh;
    width: 50%;

    h1 {
      font-family: "Karla", sans-serif;
      font-size: 3.8rem;
      color: #ce34ab;
    }

    p {
      font-family: "Roboto", sans-serif;
      font-size: 1.1rem;
      letter-spacing: 1px;
      color: #b495ad;
    }

    span {
      color: #ebc0d5;
    }
  }
}
</style>
