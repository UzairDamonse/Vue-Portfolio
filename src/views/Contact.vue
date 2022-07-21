<template>
  <div
    id="holder"
    class="pt-5 d-flex align-items-center justify-content-center"
  >
    <div class="container p-0 row" id="Contact-container">
      <div class="col-lg-6 py-5 sides">
        <h2 id="Contact-title" class="text-capitalize text-center mx-4 px-3">
          Get in touch with me
        </h2>
        <div class="row text-center mx-5 px-3 mt-2" id="Contact-left">
          <div class="col-md-6">
            <a href="https://github.com/UzairDamonse/" target="_blank">
              <i
                class="social text-decoration-none fa-brands fa-github-square my-4"
              >
              </i>
            </a>
          </div>
          <div class="col-md-6">
            <a
              href="https://www.linkedin.com/in/uzair-damonse-9b3911236/"
              target="_blank"
            >
              <i
                class="social text-decoration-none fa-brands fa-linkedin my-4"
              ></i>
            </a>
          </div>
        </div>
        <ul class="ms-3 px-3 mt-4">
          <li class="text-capitalize list-unstyled">
            <i class="fa-solid fa-location-dot py-3 pe-1"></i> location : cape
            town, south africa
          </li>
          <li class="list-unstyled">
            <i class="fa-solid fa-envelope py-3 pe-1"></i> Email :
            uzairdamonse03@gmail.com
          </li>
          <li class="text-capitalize list-unstyled">
            <i class="fa-solid fa-mobile py-3 pe-1"></i> phone number : +27 82
            601 0435
          </li>
        </ul>
      </div>
      <div class="col-lg-6 py-5 sides" id="Form">
        <div class="container d-flex justify-content-center" id="Form-Inputs">
          <form
            action="https://formspree.io/f/xnqwlvaj"
            method="POST"
            class="form pt-3"
            id="Form"
          >
            <div class="contact-name">
              <input
                type="text"
                name="Name"
                class="Form-control px-3 py-1"
                id="Name"
                placeholder="Your Name*"
                required
              />
            </div>
            <div class="contact-email">
              <input
                type="email"
                name="Email"
                class="Form-control px-3 py-1 mt-3"
                id="Email"
                placeholder="Your Email*"
                required
              />
            </div>

            <div class="subject">
              <input
                type="text"
                name="Subject"
                class="Form-control px-3 py-1 mt-3"
                id="Subject"
                placeholder="Subject*"
                required
              />
            </div>

            <div class="Message">
              <textarea
                name="Message"
                id="Message"
                cols="30"
                rows="5"
                class="Form-control mt-3 py-1 px-3"
                placeholder="Message*"
                required
              ></textarea>
            </div>
            <div class="Submit d-flex justify-content-around">
              <button
                id="send"
                type="submit"
                class="text-center rounded px-3 py-1 mt-3"
              >
                Send
              </button>
              <button
                id="reset"
                type="reset"
                class="text-center rounded px-3 py-1 mt-3"
              >
                Reset
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
  <Footer />
</template>

<script>
import Footer from "@/components/Footer.vue";
export default {
  name: "contact",
  components: {
    Footer,
  },
};
</script>

<style scoped>
#holder {
  background: url("https://i.postimg.cc/WbCM3zMg/Landing-Background.jpg");
  background-size: cover;
  background-attachment: fixed;
  height: 100vh;
}

.sides {
  box-shadow: 0px 1px 13px 2px #5f432b;
  background: linear-gradient(
    90deg,
    rgb(95, 67, 43),
    rgba(95, 67, 43, 0.552) 10%,
    rgba(192, 175, 126, 0.8) 30%,
    rgba(192, 175, 126, 0.8) 70%,
    rgb(95, 67, 43, 0.552) 90%,
    #5f432b
  );
  border: 1px solid black;
  border-radius: 20% 20% 20% 20% / 2% 5% 5% 2%;
}

#Contact-left {
  border-top: 0.1rem solid black;
  border-radius: 20% 20% 20% 20% / 2% 5% 5% 2%;
}

#Form {
  border-radius: 20% 20% 20% 20% / 5% 2% 2% 5%;
}

.social {
  font-size: 60px;
  color: var(--blue);
}

.social:hover {
  color: #325f68;
}

.form {
  width: 65%;
}

.contact-name {
  width: 100%;
}

#Name {
  width: 100%;
  border-radius: 10px;
  border: 1px solid var(--black);
}

.contact-email {
  width: 100%;
}

#Email {
  width: 100%;
  border-radius: 10px;
  border: 1px solid var(--black);
}

.Subject {
  width: 100%;
}

#Subject {
  width: 100%;
  border-radius: 10px;
  border: 1px solid var(--black);
}

.Message {
  width: 100%;
}

#Message {
  width: 100%;
  border-radius: 10px;
  border: 1px solid var(--black);
  /* box-shadow: 0px 1px 13px 2px #5f432b;
  background: rgba(192, 176, 126, 0.4); */
}

#send {
  background-color: var(--blue);
  color: var(--white);
  font-size: 1rem;
  font-weight: 650;
  border: 1px solid var(--black);
}

#send:hover {
  background-color: var(--black);
  color: var(--blue);
  border: 1px solid var(--blue);
  cursor: url("@/assets/Skyrim-normal.cur"), auto;
}

#reset {
  background-color: var(--blue);
  color: var(--white);
  font-size: 1rem;
  font-weight: 650;
  border: 1px solid var(--black);
}

#reset:hover {
  background-color: var(--black);
  color: var(--blue);
  border: 1px solid var(--blue);
  cursor: url("@/assets/Skyrim-normal.cur"), auto;
}
</style>
