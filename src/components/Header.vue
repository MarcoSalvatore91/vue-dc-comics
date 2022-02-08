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
  margin-top: 30px;
}

ul {

  li {
    margin: 0 10px;
  }

  a {
    color: black;
  }

  }

</style>
