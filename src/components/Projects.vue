<template>
  <div
    id="Holder"
    class="col-lg-4 col-md-6 col-sm-12"
    v-for="project in projects"
    :key="project.id"
  >
    <div class="cards m-3 p-3">
      <div id="project-imgs" class="d-flex justify-content-center">
        <img
          v-bind:src="project.imgURL"
          @error="aVueFunctionThatChangesTheSrc"
          id="project-img"
          alt="`${project.title}`"
        />
      </div>
      <div class="project-text">
        <h5 id="project-title">
          {{ project.title }}
        </h5>
        <p id="project-languages">
          {{ project.languages }}
        </p>
        <p id="project-description">
          {{ project.description }}
        </p>
      </div>
      <div class="icons row">
        <a
          v-bind:href="project.github"
          target="_blank"
          class="col-md-6 icon btn rounded text-decoration-none"
          ><i class="fa-brands fa-github"></i
        ></a>
        <a
          v-bind:href="project.live"
          target="_blank"
          class="col-md-6 icon btn rounded text-decoration-none"
          ><i class="fa-solid fa-link"></i
        ></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          id: "1",
          title: "Art Gallery",
          imgURL: "https://i.postimg.cc/X7ZNdjYc/art-Gallery.webp",
          github: "https://github.com/fatimagalant/art-gallery",
          live: "https://leschevresdigitalartgallery.netlify.app/",
          description:
            "This was a collaboration project to make an art gallery",
          languages: "HTML, CSS, JS, VUEJS",
        },
        {
          id: "2",
          title: "Planet Market",
          imgURL: "https://i.postimg.cc/2jtrzs7q/planet-Market.webp",
          github: "https://github.com/UzairDamonse/Planet_market",
          live: "https://wandering-star-requisitions.netlify.app/",
          description:
            "This was an assignment given to me after first learning VueJs",
          languages: "HTML, CSS, JS, VUEJS",
        },
        {
          id: "3",
          title: "Calculator",
          imgURL: "https://i.postimg.cc/59KNXYb2/Calculator.webp",
          github: "https://github.com/UzairDamonse/Calculator",
          live: "https://calculator-eg.netlify.app/",
          description:
            "This was my first project using javascript functionality",
          languages: "HTML, CSS, JS,",
        },
        {
          id: "4",
          title: "BMI Calculator",
          imgURL: "https://i.postimg.cc/RFXCQqtG/bmi-Calculator.webp",
          github: "https://github.com/UzairDamonse/BMI_calculator",
          live: "https://whats-my-bmi.netlify.app/",
          description: "This was an assignment given to me",
          languages: "HTML, CSS, JS",
        },
        {
          id: "5",
          title: "Name Search",
          imgURL: "https://i.postimg.cc/kgKnYT82/name-Search.webp",
          github: "https://github.com/UzairDamonse/AddAndFindInArray",
          live: "https://add-and-find-array.netlify.app/",
          description:
            "This was the first project that involved adding and editing to an array",
          languages: "HTML, CSS, JS",
        },
        {
          id: "6",
          title: "Restaurant",
          imgURL: "https://i.postimg.cc/rF2SzwT3/My-project-1-1.webp",
          github: "https://github.com/UzairDamonse/Restaurant",
          live: "https://restuarant-practice.netlify.app/",
          description: "This was my first project using Bootstrap",
          languages: "HTML, CSS",
        },
      ],
    };
  },
};
</script>

<style scoped>
#Holder {
  margin-bottom: 5rem;
}

.cards {
  min-height: 95%;
  margin-bottom: 5rem;
  border: #000 2px solid;
  box-shadow: inset 0px 0px 10px #000;
  background: linear-gradient(
    90deg,
    rgba(95, 67, 43),
    rgba(95, 67, 43, 0.552) 10%,
    rgba(192, 175, 126, 0.8) 30%,
    rgba(192, 175, 126, 0.8) 70%,
    rgba(95, 67, 43, 0.552) 90%,
    #5f432b
  );
}

#project-img {
  width: 100%;
  height: 80%;
}

#project-title {
  margin-top: 1rem;
  margin-bottom: 1rem;
  font-size: 2rem;
}

#project-description {
  margin-top: 1rem;
  margin-bottom: 1rem;
  font-size: 1rem;
}

#project-languages {
  margin-top: 1rem;
  margin-bottom: 1rem;
  font-size: 1.5rem;
}

.icons {
  display: flex;
  justify-content: space-around;
  margin-top: 1rem;
  margin-bottom: 1rem;
}

.icon {
  color: white;
  background-color: var(--blue);
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40%;
  font-size: 1.5rem;
}

.icon:hover {
  color: var(--blue);
  background-color: var(--white);
}
</style>
