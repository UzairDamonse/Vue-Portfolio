<template>
  <div id="landing">
    <h1 id="Sub-title" class="text-capitalize">aspiring developer</h1>
    <h1 id="Name" class="text-capitalize">uzair damonse</h1>
  </div>
  <Footer />
</template>

<script>
import Footer from "./Footer.vue";
export default {
  name: "HelloWorld",
  components: {
    Footer,
  },
};
</script>

<style scoped>
#landing {
  height: 100vh;
  background: url("https://i.postimg.cc/WbCM3zMg/Landing-Background.jpg");
  background-size: cover;
  background-attachment: fixed;
  text-align: center;
  padding: 26vh 31vw;
  align-items: center;
}

#Name {
  font-size: 5.5rem;
  font-weight: 500;
  border-top: 0.2rem solid black;
  border-radius: 31% 30% 30% 31% / 4% 4% 0% 0%;
  font-family: skyrim;
  background-color: #000 !important;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  background-clip: text;
  color: transparent;
  text-shadow: 0px 3px 3px var(--white);
}

#Sub-title {
  font-size: 3.5rem;
  font-weight: 500;
  font-family: elder;
  background-color: #000 !important;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  background-clip: text;
  color: transparent;
  text-shadow: 0px 3px 3px var(--white);
}

@media only screen and (max-width: 550px) {
  #Name{
    font-size: 4rem;
  }

  #Sub-title{
    font-size: 3rem;
  }
}

@media only screen and (max-width: 480px) {
  #Name{
    font-size: 3rem;
  }

  #Sub-title{
    font-size: 2rem;
  }
}
@media only screen and (max-width: 480px) {
  #Name{
    font-size: 2.5rem;
  }

  #Sub-title{
    font-size: 1.5rem;
  }
}
</style>
