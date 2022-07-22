<template>
  <div id="Projects">
    <div
      class="container py-5 border edge bg-dark"
      data-aos="fade-up"
      data-aos-duration="900"
    >
      <h2 id="Project-title" class="text-start mx-4 px-4">
        Some of my projects
      </h2>
      <p class="underline text-start mx-4 px-3 mb-5"></p>

      <p class="description mb-5 text-start mx-4 px-4">
        These are some of the projects I have worked on so far.
      </p>
      <div id="ProjectSlider" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-indicators mt-5 pt">
          <button
            type="button"
            data-bs-target="#ProjectSlider"
            data-bs-slide-to="0"
            class="active rounded-circle ms-2"
            style="width: 25px; height: 25px"
            aria-current="true"
            aria-label="Slide 1"
          ></button>
          <button
            type="button"
            data-bs-target="#ProjectSlider"
            data-bs-slide-to="0"
            class="active rounded-circle ms-2"
            style="width: 25px; height: 25px"
            aria-current="true"
            aria-label="Slide 2"
          ></button>
          <button
            type="button"
            data-bs-target="#ProjectSlider"
            data-bs-slide-to="0"
            class="active rounded-circle ms-2"
            style="width: 25px; height: 25px"
            aria-current="true"
            aria-label="Slide 3"
          ></button>
          <button
            type="button"
            data-bs-target="#ProjectSlider"
            data-bs-slide-to="0"
            class="active rounded-circle ms-2"
            style="width: 25px; height: 25px"
            aria-current="true"
            aria-label="Slide 4"
          ></button>
          <button
            type="button"
            data-bs-target="#ProjectSlider"
            data-bs-slide-to="1"
            aria-label="Slide 5"
            class="rounded-circle ms-2"
            style="width: 25px; height: 25px"
          ></button>
          <button
            type="button"
            data-bs-target="#ProjectSlider"
            data-bs-slide-to="2"
            aria-label="Slide 6"
            class="rounded-circle ms-2"
            style="width: 25px; height: 25px"
          ></button>
        </div>
        <div class="carousel-inner" id="test-img">
          <div class="carousel-item pb-5 mb-5 text-center active">
            <img
              src="https://i.postimg.cc/FsXxfDSB/artGallery.png"
              id="Dream-destination"
              class="d-block rounded"
              alt="Dream-destination"
            />
            <div class="carousel-caption mb-4 text-dark">
              <h5 class="Dream-destination-text">Art Gallery</h5>
              <p class="Dream-destination-text">HTML, CSS, JS, VUEJS</p>
              <div class="links m-3">
                <a
                  href="https://github.com/fatimagalant/art-gallery"
                  target="_blank"
                  class="project-links btn rounded-pill text-decoration-none"
                  ><i class="fa-brands fa-github"></i> GitHub</a
                >
                <a
                  href="https://leschevresdigitalartgallery.netlify.app/"
                  target="_blank"
                  class="project-links btn rounded-pill text-decoration-none"
                  ><i class="fa-solid fa-link"></i> Live</a
                >
              </div>
              <Projects />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <CCarousel controls indicators>
    <CCarouselItem>
      <img class="d-block w-100" src="/images/vue.jpg" alt="slide 1" />
      <CCarouselCaption class="d-none d-md-block">
        <h5>First slide label</h5>
        <p>Some representative placeholder content for the first slide.</p>
      </CCarouselCaption>
    </CCarouselItem>
    <CCarouselItem>
      <img class="d-block w-100" src="/images/react.jpg" alt="slide 2" />
      <CCarouselCaption class="d-none d-md-block">
        <h5>First slide label</h5>
        <p>Some representative placeholder content for the first slide.</p>
      </CCarouselCaption>
    </CCarouselItem>
    <CCarouselItem>
      <img class="d-block w-100" src="/images/angular.jpg" alt="slide 3" />
      <CCarouselCaption class="d-none d-md-block">
        <h5>First slide label</h5>
        <p>Some representative placeholder content for the first slide.</p>
      </CCarouselCaption>
    </CCarouselItem>
  </CCarousel>
  <Footer />
</template>

<script>
import Footer from "@/components/Footer.vue";
import Projects from "@/components/Projects.vue";
import { CAlert } from "@coreui/vue";
import CCarousel from "@coreui/vue/src/components/carousel/CCarousel";

export default {
  components: {
    Footer,
    Projects,
    CCarousel,
  },
};
</script>

<style scoped>
#Projects {
  min-height: 100vh;
  background-color: var(--black);
}

#Projects .container {
  background-color: var(--grey);
  box-shadow: 0px 1px 13px 8px #434141;
}

#Project-title {
  font-size: 50px;
}

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
