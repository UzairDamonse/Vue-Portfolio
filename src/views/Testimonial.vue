<template>
  <div id="Testmonial-container">
    <div class="testimonials">
      <h1 id="title">Testimonials</h1>
      <Testimonials />
    </div>
  </div>
  <Footer />
</template>

<script>
import Footer from "@/components/Footer.vue";
import Testimonials from "@/components/Testimonials.vue";

export default {
  components: {
    Footer,
    Testimonials,
  },
};
</script>

<style scoped>
* {
  color: var(--white);
}
#Testmonial-container {
  background: url(https://i.postimg.cc/J0gz6gqj/testimonial-back.jpg);
  background-attachment: fixed;
  background-size: cover;
  min-height: 100vh;
}

.testimonials {
  padding-top: 5rem;
  padding-bottom: 5rem;
}

#title {
  font-family: skyrim;
  font-size: 5rem;
  color: var(--blue);
}
</style>
