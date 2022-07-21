<template>
  <div id="about">
    <div class="about-container container py-5">
      <h2 class="about-title text-start mx-4 px-4">
        <span id="Name">Hi, I'm Uzair </span>, a prospective full-stack
        developer who likes a challenge
      </h2>
      <p class="description mx-4 px-4 mt-4">
        I am a young developer that has a passion for learning as well as
        teaching, as I have experience with both by being a part of a volunteer
        organisation called St. John. I am an outspoken, self-confident person
        that enjoys competition and sharing knowledge and experiences with
        like-minded people. I get my passion for coding from gaming most notably
        The Elder Scrolls V: Skyrim where I have accumulated a considerable
        amount of hours
      </p>
      <div id="cardHolder" class="row d-flex justify-content-around">
        <div id="cardTitle">
          <h1 class="mt-2" id="Skills">Skills</h1>
        </div>
        <div id="card" class="col-md-4">
          <i id="html" class="skill-icons fa-brands fa-html5"></i>
        </div>
        <div id="card" class="col-md-4">
          <i id="css" class="skill-icons fa-brands fa-css3"></i>
        </div>
        <div id="card" class="col-md-4">
          <i id="js" class="skill-icons fa-brands fa-js"></i>
        </div>
        <div id="card" class="col-md-4">
          <i id="vuejs" class="skill-icons fa-brands fa-vuejs"></i>
        </div>
        <div id="card" class="col-md-4">
          <i id="mySql" class="skill-icons fa-solid fa-database"></i>
        </div>
        <div id="card" class="col-md-4">
          <i id="bootstrap" class="skill-icons fa-brands fa-bootstrap"></i>
        </div>
        <div id="card" class="col-md-4">
          <i id="node-js" class="skill-icons fa-brands fa-node-js"></i>
        </div>
        <div id="card" class="col-md-4">
          <i id="git" class="skill-icons fa-brands fa-git-square"></i>
        </div>
      </div>
      <div id="Resume" v-for="resume in resume" :key="resume.id"></div>
    </div>
  </div>
  <Footer />
</template>

<script>
import Footer from "@/components/Footer.vue";
export default {
  data() {
    return {
      resume: [
        {
          id: 1,
          Title: "ATK Arena",
          Role: "Intern",
          Year: "December 2021-January 2022",
          Description: "",
        },
        {
          id: 2,
          Title: "Cape Academy of Maths, Science and Technology",
          Role: "Matric",
          Year: "2017-2021",
          Description:
            "I matriculated in 2021 where I graduated with a dipolma",
        },
        {
          id: 3,
          Title: "Life Choices",
          Role: "Student",
          Year: "March 2022-Present",
          Description:
            "I am attending a full-time coding course where I am being taught to become a full-stack web developer",
        },
      ],
    };
  },
  components: {
    Footer,
  },
};
</script>

<style scoped>
/* About */

#about {
  background: url("https://i.postimg.cc/sxrxFbrK/About-background-1.jpg");
  min-height: 100vh;
  background-size: cover;
  background-attachment: fixed;
  color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-shadow: 0px 0px 5px #000;
}

.about-container {
  margin-top: 5rem;
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

.about-title {
  font-size: 2.5rem;
}

#Name {
  color: var(--blue);
}

.description {
  font-size: 1.4rem;
}

#Skills {
  font-family: skyrim;
  font-size: 5rem;
}

#cardHolder {
  margin-bottom: 2rem;
}

#card {
  background: url("https://i.postimg.cc/VL8QjPHF/My-project-3.png");
  background-size: cover;
  height: 22rem;
  width: 22rem;
  margin-top: 4rem;
}

#cardTitle {
  color: var(--blue);
  text-shadow: 0px 0px 2px #000;
}

.skill-icons {
  font-size: 11rem;
  color: rgba(106, 102, 92, 0.8);
  text-shadow: 0px 0px 8px rgba(79, 73, 67, 0.8);
}

#html {
  padding-top: 5.5rem;
  padding-left: 0.7rem;
}
#css {
  padding-top: 5.7rem;
  padding-left: 1.3rem;
}
#js {
  padding-top: 5.35rem;
  padding-right: 0.1rem;
}
#vuejs {
  padding-top: 6.3rem;
  padding-left: 1rem;
}
#mySql {
  padding-top: 5.2rem;
  padding-left: 0.4rem;
}
#bootstrap {
  padding-top: 5.4rem;
  padding-left: 0.6rem;
}
#node-js {
  padding-top: 5.5rem;
  padding-left: 0.5rem;
}

#git {
  padding-top: 5.4rem;
  padding-left: 0.2rem;
}
</style>
