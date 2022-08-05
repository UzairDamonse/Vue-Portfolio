<template>
  <nav id="NavBar">
    <div class="toggle" id="toggle">
      <i class="fas fa-bars menu mx-1" @click="toggleNav()"></i>
    </div>

    <ul id="list">
      <div>
        <li class="Links">
          <div class="link">
            <audio ref="song" :src="songs.src" autoplay loop></audio>
            <a class="MusicButton" v-if="!isPlaying" @click="play" title="Play"
              ><i class="fa-solid fa-volume-xmark"></i
            ></a>
            <a class="MusicButton" v-else @click="pause" title="Pause"
              ><i class="fa-solid fa-volume-high"></i
            ></a>
          </div>
        </li>
      </div>
      <li class="Links">
        <router-link to="/" class="link" @click="toggleNav()">Home</router-link>
      </li>
      <li class="Links">
        <router-link @click="toggleNav()" to="/about" class="link"
          >About</router-link
        >
      </li>
      <li class="Links">
        <router-link @click="toggleNav()" to="/projects" class="link"
          >Projects</router-link
        >
      </li>
      <li class="Links">
        <router-link @click="toggleNav()" to="/testimonial" class="link"
          >Testimonials</router-link
        >
      </li>
      <li class="Links">
        <router-link @click="toggleNav()" to="/contact" class="link"
          >Contact</router-link
        >
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      index: 0,
      isPlaying: true,
      songs: {
        src: require("../assets/A-mystical-journey-3.mp3"),
      },
      player: new Audio(),
    };
  },
  methods: {
    play(song) {
      this.$refs.song.play();
      this.isPlaying = true;
    },
    pause() {
      this.$refs.song.pause();
      this.isPlaying = false;
    },
    toggleNav() {
      document.getElementById("list").classList.toggle("active");
    },
  },
  created() {
    this.player.src = this.songs.src;
  },
  mounted() {},
};
</script>

<style scoped>
/* CSS Reset */

* {
  scroll-behavior: smooth;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

nav {
  position: fixed;
  width: 100%;
  height: 0;
  background-color: rgba(0, 0, 0, 0.5);
  top: 0;
}

ul {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  background-color: rgba(0, 0, 0, 0.5);
  z-index: 100000000;
}

ul li {
  list-style: none;
  margin: 1.5rem;
}

ul li a {
  color: #fff;
  text-decoration: none;
  padding: 1.5rem;
  font-size: 1.2rem;
  font-family: skyrim;
}

.MusicButton {
  color: #fff;
  text-decoration: none;
  padding: 1.5rem;
  font-size: 1.2rem;
  font-family: skyrim;
}

.menu {
  padding: 0.9rem 0.7rem;
  margin: 0.2rem 0.2rem;
}

a:hover {
  background-color: rgba(207, 194, 199, 0.5);
}

.toggle {
  width: 100%;
  background-color: rgba(0, 0, 0, 0.3);
  color: #fff;
  font-size: 2.5rem;
  display: flex;
  justify-content: flex-end;

  display: none;
}

@media (max-width: 896px) {
  .toggle {
    display: flex;
  }

  .menu:hover {
    background-color: rgba(207, 194, 199, 0.5);
  }

  ul {
    flex-direction: column;
    width: 100%;
    position: relative;
    top: -100vh;
    transition: all 0.7s ease-in;
  }

  .menu {
    z-index: 100000000;
  }

  .active {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 94vh;
    top: 0vh;
  }
}
</style>
