<template>
  <section id="projects">
    <div class="container">
      <h1>/ Projects</h1>
      <ul class="project-list">
        <li
          class="list-item"
          v-for="project in projects"
          :key="project.title"
          data-aos="fade-right"
          data-aos-duration="1600"
          data-aos-easing="ease"
          data-aos-once="false"
          data-aos-delay="200"
        >
          <div class="list-content">
            <h2>
              <strong>{{ project.title }}</strong>
            </h2>
            <p>{{ project.desc }}</p>
            <a v-bind:href="'' + project.link" target="_blank">
              <img class="git-logo" :src="gitLogo" />
            </a>
          </div>
          <img :src="project.imagePath" />
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      gitLogo: require("../assets/github/GitHub-Mark-Light-120px-plus.png"),
      projects: [
        {
          title: "Lindcode tutorials learning platform",
          desc: "A Fullstack web app built in React.js with Javascript, SCSS and Axios consuming a Rest-API built with MongoDB on Railway, Mongoose, NodeJs and ExpressJs",
          imagePath: require("../assets/lindcode/tutorial.png"),
        },
        {
          title: "Desserts & Cocktails Recipe Collection",
          desc: "A Fullstack Recipe collection site built in React.js with Typescript, consuming a Rest-API built with NodeJs, Express and MongoDB. Backend deployed to Heroku and MongoDB Atlas while Frontend on Netlify.",
          link: "https://github.com/StellaSFE96/Recipe-site-React",
          imagePath: require("../assets/recipes/recipe.png"),
        },
        {
          title: "Sinus Webshop",
          desc: "Sinus webshop is an online store built in Vue.js, Vuex and Vue Router with common features like add/ remove items in cart, checkout, register user or shop as a guest.",
          link: "https://github.com/StellaSFE96/sinus-webshop",
          imagePath: require("../assets/sinus/products.png"),
        },
        {
          title: "E-wallet App",
          desc: "A single page application built in Vue.js with user options such as add new cards and view active card in card stack. Includes two views which shows home with added cards and second view for add new card.",
          link: "https://github.com/StellaSFE96/E-wallet",
          imagePath: require("../assets/e-wallet/home.png"),
        },
        {
          title: "Star Wars Catalog",
          desc: "Star Wars catalog is a single page application built with HTML, CSS, Javascript using the Star Wars API to list characters and their information.",
          link: "https://github.com/StellaSFE96/JavaScript-projekt?organization=StellaSFE96&organization=StellaSFE96",
          imagePath: require("../assets/starWars/starwars.png"),
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#projects {
  padding: 7rem;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  .container {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 80%;

    img {
      width: 40%;
      border-radius: 6px;
      margin-left: 2rem;
      transition: transform 300ms ease-in-out;
      cursor: pointer;

      &:hover {
        transform: scale(1.2);
      }
    }

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

    .git-logo {
      background-color: #4a154e;
      width: 5%;
      margin: 3rem 0 0 0;

      &:hover {
        transform: translateY(-5px);
      }
    }
  }

  .project-list {
    width: 100%;
    height: auto;
    margin-top: 1rem;
    list-style: none;

    h2 {
      font-family: "karla", sans-serif;
      color: #ebc0d5;
    }

    p {
      margin-top: 1rem;
    }

    .list-item {
      margin-top: 2rem;
      display: flex;
      justify-content: space-between;

      &:hover {
        transform: translateY(-5px);
      }
    }

    .list-content {
      padding: 20px;
      width: 60%;
      border-radius: 6px;
    }

    .list-content,
    h2,
    strong,
    p {
      background-color: #4a154e;
    }
  }
}

@media only screen and (min-width: 370px) and (max-width: 1100px) {
  #projects {
    padding: 8rem 0 0 0;

    .container {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      align-items: center;
      width: 100%;

      img {
        margin: 20px 0px 0 0;
        min-width: 90%;
        height: auto;
        border-radius: 6px;
        transition: transform 300ms ease-in-out;
        cursor: pointer;

        &:hover {
          transform: scale(1.2);
        }
      }

      h1 {
        font-size: 3rem;
      }

      p {
        font-size: 1.1rem;
      }

      .git-logo {
        min-width: 1.6rem;
        margin: 3rem 0 0 0.8rem;

        &:hover {
          transform: translateY(-5px);
        }
      }
    }

    .project-list {
      width: 100%;
      height: auto;
      margin-top: 1rem;
      list-style: none;

      p {
        margin-top: 1rem;
      }

      .list-item {
        margin-top: 2rem;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
      }

      .list-content {
        padding: 5px;
        min-width: 90%;
        border-radius: 6px;
      }
    }
  }
}
</style>
