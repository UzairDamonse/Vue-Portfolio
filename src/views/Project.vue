<template>
  <Footer />
</template>

<script>
import Footer from "@/components/Footer.vue";

export default {
  data() {
    return {
      projects: [
        {
          id: 1,
          Title: "Restaurant",
          GitHub: "https://github.com/UzairDamonse/Restaurant",
          Live: "https://restuarant-practice.netlify.app/",
          Description:
            "This project was my firt project that included everything I learned with Bootstrap",
        },
        {
          id: 2,
          Title: "Dream-destination",
          GitHub: "https://github.com/UzairDamonse/DreamDestinationV2",
          Live: "https://dream-destination-v2.netlify.app/",
          Description:
            "This project was my firt project that included HTML and CSS",
        },
        {
          id: 3,
          Title: "Calculator",
          GitHub: "https://github.com/UzairDamonse/Calculator",
          Live: "https://calculator-eg.netlify.app/",
          Description:
            "This project was my firt project that included flexbox as well as Javscript functionality",
        },
      ],
    };
  },
  components: {
    Footer,
  },
};
</script>

<style></style>
