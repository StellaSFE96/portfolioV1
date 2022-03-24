<template>
  <section id="experience">
    <div class="container">
      <h1>/ Experience</h1>
      <p>
        Some of the main technologies i have come to learn and implement while
        building school projects are <span>Vanilla JavaScript</span> and
        <span>Vue.js</span>. Below are some more i have been working with:
      </p>
    </div>
    <div class="skills">
      <ul class="skill-list">
        <li
          class="list-item"
          v-for="skill in skills"
          :key="skill.name"
          data-aos="fade-right"
          data-aos-duration="1600"
          data-aos-easing="ease"
          data-aos-once="false"
          data-aos-delay="200"
        >
          <img :src="skill.arrow" alt="arrow" />
          <p>{{ skill.name }}</p>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  props: ["skills"],
};
</script>

<style lang="scss" scoped>
#experience {
  height: 100vh;
  padding-top: 10px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  .skills {
    margin-top: 50px;
    height: auto;
    width: 50%;
    color: #ebc0d5;

    img {
      width: 8px;
      height: 15px;
      margin-right: 10px;
    }

    .skill-list {
      margin: 20px;
      display: grid;
      grid-template-columns: repeat(2, 1fr);
    }

    .list-item {
      display: flex;
      margin-bottom: 20px;
      font-family: "Karla", sans-serif;
    }
  }

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

@media only screen and (min-width: 370px) and (max-width: 770px) {
  #experience {
    padding: 1vh;
    .skills {
      width: 90%;

      .skill-list {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        width: 350px;
        margin: 0px;
      }

      .list-item {
        display: flex;
        padding-right: 50px;
      }
    }

    .container {
      width: 100%;

      h1 {
        font-size: 3rem;
      }
    }
  }
}
</style>
