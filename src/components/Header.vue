<template>
  <div id="header">

    <!-- Nav Bar -->
    <div id="top-header"></div>
    <section id="nav-bar" class="bg-white d-flex">
      <div class="container">
        <img src="../assets/img/dc-logo.png" alt="Logo">
      </div>
      <div class="container">
        <!--  TO DO CHANGE WITH CICLE -->
        <ul class="d-flex">
          <li v-for="link in links" :key="link.text">
            <a :href="link.url" :class="{ active: link.active }">{{ link.text }}</a>
          </li>
        </ul>
      </div>
    </section>

  </div>
</template>

<script>

export default {
  name: 'Header',
  data() {
    return {
      links: [
        { text: "CHARACTERS", url: "#", active: true,},
        { text: "COMICS", url: "#", active: false,},
        { text: "MOVIES", url: "#", active: false,},
        { text: "TV", url: "#", active: false,},
        { text: "GAMES", url: "#", active: false,},
        { text: "COLLECTIBLES", url: "#", active: false,},
        { text: "VIDEOS", url: "#", active: false,},
        { text: "FANS", url: "#", active: false,},
        { text: "NEWS", url: "#", active: false,},
        { text: "SHOP", url: "#", active: false,},
      ]
    }
  }
}

</script>

<style scoped lang='scss'>

@import '../assets/sass/style.scss';

#top-header {
  height: 30px;
  background-color: black;
}

#nav-bar {
  height: 150px;
  align-items: center;
}

ul {

  li {
    margin: 0 10px;
    height: 150px;
    &:hover {
      border-bottom: 5px solid rgb(2,130,249);
    }
    }

  a {
    color: black;
    font-weight: bold;
    line-height: 150px;
    &.active {
      color: rgb(2,130,249);
    }
  }

  }

</style>
