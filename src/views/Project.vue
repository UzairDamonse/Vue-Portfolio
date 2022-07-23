<template>
  <div id="Projects">
    <h1 id="title">
      Some of my projects
    </h1>
    <div class="row">
      <Projects/>
    </div>
  </div>
  <Footer />
</template>

<script>
import Footer from "@/components/Footer.vue";
import Projects from "@/components/Projects.vue";
export default {
  components: {
    Footer,
    Projects,
  },
};
</script>

<style scoped>
#Projects {
  min-height: 100vh;
  background: url('https://i.postimg.cc/zvwk7KpF/project-background.jpg');
  background-attachment: fixed;
  background-size: cover;
  color: #fff;
  text-shadow: 0px 0px 5px #000;
  overflow-x: hidden;

}

#title {
  padding-top: 5rem;
  font-family: skyrim;
  font-size: 5rem;
  color: var(--blue);
  text-align: center;
}

.row {
  padding-top: 5rem;
}
</style>
