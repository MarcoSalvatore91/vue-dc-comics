<template>
  <div id="header">

    <!-- Nav Bar -->
    <section id="nav-bar" class="bg-white d-flex">
      <div class="container">
        <img src="../assets/img/dc-logo.png" alt="Logo">
      </div>
      <div class="container">
        <!--  TO DO CHANGE WITH CICLE -->
        <ul class="d-flex">
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#">COMICS</a></li>
          <li><a href="#">MOVIES</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">GAMES</a></li>
          <li><a href="#">COLLECTIBLES</a></li>
          <li><a href="#">VIDEOS</a></li>
          <li><a href="#">FANS</a></li>
          <li><a href="#">NEWS</a></li>
          <li><a href="#">SHOP</a></li>
        </ul>
      </div>
    </section>

    <!-- Contents -->
    <section id="contents">
      <div class="container">
        <h2 class="color-white">-- Content goes here --</h2>
      </div>
    </section>

  </div>
</template>

<script>


export default {
  name: 'Header',
  
}
</script>

<style scoped lang='scss'>

@import '../assets/sass/style.scss';

#nav-bar {
  height: 150px;
  margin: 10px 0;
}

#contents {
  height: 150px;
}

ul {

  li {
    list-style-type: none;
    margin: 0 10px;
  }

  a {
    font-size: 0.8rem;
    color: black;
    text-decoration: none;
  }

  }

  h2 {
    line-height: 150px;
  }

</style>
