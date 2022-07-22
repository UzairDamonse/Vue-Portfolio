<template>
  <div v-for="resume in resume" :key="resume.id">
    <p class="underline text-start mx-4 px-3 mb-5"></p>
    <h3 class="text-start mx-4 px-3 text">{{ resume.Title }}</h3>
    <h4 class="text-start mx-4 px-3 text">{{ resume.Role }}</h4>
    <h5 class="text-start mx-4 px-3 text">{{ resume.Year }}</h5>
    <p class="text-start mx-4 px-3 pb-3">{{ resume.Description }}</p>
  </div>
</template>

<script>
export default {
  name: "resume",
  data() {
    return {
      resume: [
        {
          id: 1,
          Title: "ATK Arena",
          Role: "Intern",
          Year: "December 2021-January 2022",
          Description:
            "I worked at ATK Arena during the December holidays of 2021 as an intern where I was responsible for customer service as well as helping with any technical problems customers faced.",
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
};
</script>

<style scoped>
p {
  font-size: 1.2rem;
}

.text {
  margin-bottom: 0.75rem;
}
</style>
