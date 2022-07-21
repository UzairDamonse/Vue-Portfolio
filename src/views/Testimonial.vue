<template>
  <Footer />
</template>

<script>
import Footer from "@/components/Footer.vue";

export default {
  data() {
    return {
      testimonial: [
        {
          id: 1,
          Title: "Jason Wandrag",
          Role: "Lecturer",
          imgURL: "https://i.postimg.cc/kXKQK41t/Jason.jpg",
          Description:
            "The best way to describe Uzair is to think of a big, cuddly teddy bear. Uzair manages to bring light to any situation with his infectious smile and very warm and caring demeanor. Uzair has also managed to rapidly upskill in software development, which makes him a perfect candidate for any software development role.",
        },
        {
          id: 2,
          Title: "Sandy Williams",
          Role: "Lecturer",
          imgURL: "https://i.postimg.cc/NfqTstsG/Sandy.jpg",
          Description: `Uzair Damonse joined St John Brigade in the year 2014. He then became a member of the brigade and volunteered his time to helping others in need. Uzair is a valued member of the St John Brigade and has contributed a lot of his time as a volunteer. Uzair is a hardworking, determined, and intelligent young man...`,
        },
        {
          id: 3,
          Title: "Ricardo Ronan Moses",
          Role: "Peer",
          imgURL: "https://i.postimg.cc/P5qqhVwr/Ricardo.jpg",
          Description: `Uzair Damonse is a very animated young man who is never afraid to express his thoughts while keeping other people's thoughts and feeling in mind . He has the ability to communicate clearly when working with a group and has an excellent ability to ensure the project reaches it's desired outcome.`,
        },
        {
          id: 4,
          Title: "Fatima Gallant",
          Role: "Peer",
          imgURL: "https://i.postimg.cc/ZqC0PsbD/Fatima.jpg",
          Description:
            "Uzair is a fast learner with the ability to pick up new skills swiftly. With a natural ability for all things technical, Uzair will find a way to fix any problem and overcome any challenge. His competitive nature helps him to exceed in his field. It's been an absolute pleasure working alongside such a bright-minded guy.",
        },
        {
          id: 5,
          Title: "Jesse Spence",
          Role: "Peer",
          imgURL: "https://i.postimg.cc/gJ7JBVJk/Jesse.jpg",
          Description:
            "Uzair is an extremely intelligent individual, he is clearly able to grasp complex problems faster than the average person. He has a keen eye for detail and diligently works toward perfection. He's also kind and open-minded which makes him an absolute delight to be around.",
        },
        {
          id: 6,
          Title: "Carla Amy Lawrence",
          Role: "Peer",
          imgURL: "https://i.postimg.cc/bY2kfrjF/Carla.jpg",
          Description:
            "Uzair Damonse is an excellent web developer. His friendly disposition and vast skills makes him an asset to any team. Uzair's work is consistently displayed in both a creative and professional manner. His vision translates beautifully to ensure a well crafted user interface and functional user experience.",
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
