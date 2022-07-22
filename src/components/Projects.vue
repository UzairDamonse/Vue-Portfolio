<template>
  <div
    class="carousel-item pb-5 mb-5 text-center"
    v-for="project in projects"
    :key="project.id"
  >
    <img
      v-bind:src="project.imgURL"
      id="Dream-destination"
      class="d-block rounded"
      alt="Dream-destination"
    />
    <div class="carousel-caption mb-4 text-dark">
      <h5 class="Dream-destination-text">
        {{ project.title }}
      </h5>
      <p class="Dream-destination-text">
        {{ project.description }}
      </p>
      <div class="links m-3">
        <a
          v-bind:href="project.github"
          target="_blank"
          class="project-links btn rounded-pill text-decoration-none"
          ><i class="fa-brands fa-github"></i> GitHub</a
        >
        <a
          v-bind:href="project.live"
          target="_blank"
          class="project-links btn rounded-pill text-decoration-none"
          ><i class="fa-solid fa-link"></i> Live</a
        >
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
          title: "Planet Market",
          imgURL: "https://i.postimg.cc/dVqm634R/planetMarket.png",
          github: "https://github.com/UzairDamonse/Planet_market",
          live: "https://wandering-star-requisitions.netlify.app/",
          description: "HTML, CSS, JS, VUEJS",
        },
        {
          id: "2",
          title: "Calculator",
          imgURL: "https://i.postimg.cc/nhtwJnTM/Calculator.png",
          github: "https://github.com/UzairDamonse/Calculator",
          live: "https://calculator-eg.netlify.app/",
          description: "HTML, CSS, JS,",
        },
        {
          id: "3",
          title: "BMI Calculator",
          imgURL: "https://i.postimg.cc/mrmdCC4F/bmiCalculator.png",
          github: "https://github.com/UzairDamonse/BMI_calculator",
          live: "https://whats-my-bmi.netlify.app/",
          description: "HTML, CSS, JS",
        },
        {
          id: "4",
          title: "Name Search",
          imgURL: "https://i.postimg.cc/vTfLq6Jh/nameSearch.png",
          github: "https://github.com/UzairDamonse/AddAndFindInArray",
          live: "https://add-and-find-array.netlify.app/",
          description: "HTML, CSS, JS",
        },
        {
          id: "5",
          title: "Restaurant",
          imgURL: "https://i.postimg.cc/5N5S8LqN/Restaurant.png",
          github: "https://github.com/UzairDamonse/Restaurant",
          live: "https://restuarant-practice.netlify.app/",
          description: "HTML, CSS,",
        },
      ],
    };
  },
};
</script>

<style>
#Dream-destination {
  width: 90%;
  margin: auto;
  box-shadow: 3px 4px 18px 5px rgba(0, 0, 0, 0.7);
}
.Dream-destination-text {
  text-shadow: 1px 1px 6px rgba(191, 191, 191, 0.84);
}

#Calculator {
  width: 90%;
  margin: auto;
  box-shadow: 3px 4px 18px 5px rgba(0, 0, 0, 0.7);
}

.Calculator-text {
  text-shadow: 1px 1px 6px rgba(191, 191, 191, 0.84);
}

#Restaurant {
  width: 90%;
  margin: auto;
  box-shadow: 3px 4px 18px 5px rgba(0, 0, 0, 0.7);
}
.Restaurant-text {
  text-shadow: 1px 1px 6px rgba(191, 191, 191, 0.84);
}

.project-links {
  color: var(--blue);
  background-color: var(--grey);
}

.project-links:hover {
  color: var(--grey);
  background-color: var(--blue);
}
</style>
