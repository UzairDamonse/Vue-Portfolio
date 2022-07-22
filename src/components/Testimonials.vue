<template>
  <div v-for="testimonial in testimonial" :key="testimonial.id" class="mx-3">
    <img id="testImg" class="my-4 pt-5" v-bind:src="testimonial.imgURL" />
    <h2>{{ testimonial.Title }}</h2>
    <h3 id="Role">{{ testimonial.Role }}</h3>
    <p>
      <i class="fa-solid fa-quote-left"></i> {{ testimonial.Description }}
      <a v-if="testimonial.URL" v-bind:href="testimonial.URL" target="_blank"
        >Read more</a
      >
      <i class="fa-solid fa-quote-right"></i>
    </p>
  </div>
</template>

<script>
export default {
  name: "Testimonials",
  data() {
    return {
      testimonial: [
        {
          id: 1,
          Title: "Jason Wandrag",
          Role: "Lecturer",
          imgURL: "https://i.postimg.cc/YSkpVX2J/Jason-removebg-preview.png",
          Description:
            "The best way to describe Uzair is to think of a big, cuddly teddy bear. Uzair manages to bring light to any situation with his infectious smile and very warm and caring demeanor. Uzair has also managed to rapidly upskill in software development, which makes him a perfect candidate for any software development role.",
        },
        {
          id: 2,
          Title: "Sandy Williams",
          Role: "Lecturer",
          imgURL: "https://i.postimg.cc/4ND4vfD4/Sandy-removebg-preview.png",
          URL: "https://docs.google.com/document/d/e/2PACX-1vSc17zLpRIZ4s1bm1SKTKwW7pwmhfRQ-pAIQmFvwB1qi6HijWivRAys147AyBr2QEdf_FrVTmOgRqJM/pub",
          Description: `Uzair Damonse joined St John Brigade in the year 2014. He then became a member of the brigade and volunteered his time to helping others in need. Uzair is a valued member of the St John Brigade and has contributed a lot of his time as a volunteer. Uzair is a hardworking, determined, and intelligent young man...`,
        },
        {
          id: 3,
          Title: "Ricardo Ronan Moses",
          Role: "Peer",
          imgURL: "https://i.postimg.cc/269r1rdD/Ricardo-removebg-preview.png",
          Description: `Uzair Damonse is a very animated young man who is never afraid to express his thoughts while keeping other people's thoughts and feeling in mind . He has the ability to communicate clearly when working with a group and has an excellent ability to ensure the project reaches it's desired outcome.`,
        },
        {
          id: 4,
          Title: "Fatima Gallant",
          Role: "Peer",
          imgURL: "https://i.postimg.cc/SsxmQJMd/Fatima-removebg-preview.png",
          Description:
            "Uzair is a fast learner with the ability to pick up new skills swiftly. With a natural ability for all things technical, Uzair will find a way to fix any problem and overcome any challenge. His competitive nature helps him to exceed in his field. It's been an absolute pleasure working alongside such a bright-minded guy.",
        },
        {
          id: 5,
          Title: "Jesse Spence",
          Role: "Peer",
          imgURL: "https://i.postimg.cc/mg7Lmx4Y/Jesse-removebg-preview.png",
          Description:
            "Uzair is an extremely intelligent individual, he is clearly able to grasp complex problems faster than the average person. He has a keen eye for detail and diligently works toward perfection. He's also kind and open-minded which makes him an absolute delight to be around.",
        },
        {
          id: 6,
          Title: "Carla Amy Lawrence",
          Role: "Peer",
          imgURL: "https://i.postimg.cc/jjXsrzLC/Carla-removebg-preview.png",
          Description:
            "Uzair Damonse is an excellent web developer. His friendly disposition and vast skills makes him an asset to any team. Uzair's work is consistently displayed in both a creative and professional manner. His vision translates beautifully to ensure a well crafted user interface and functional user experience.",
        },
      ],
    };
  },
};
</script>

<style scoped>
* {
  color: var(--white);
  text-shadow: 0px 0px 20px #757674;
}
.testimonials {
  padding-top: 5rem;
  padding-bottom: 5rem;
}

p {
  font-size: 1.2rem;
}

#testImg {
  height: 300px;
  width: 300px;
  filter: drop-shadow(0px 0px 5px #757674);
}

#Role {
  color: var(--blue);
}

a {
  color: var(--blue);
}

a:hover {
  color: var(--white);
}
</style>
