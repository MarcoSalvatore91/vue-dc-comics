<template>
  <div class="footer">
    <section class="d-flex container">
      <!-- # TO DO CHANGE -->
      <div>
        <ul>
          <li><a href="#"><h4>DC COMICS</h4></a></li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Characters</a></li>
        </ul>
      </div>

      <div class="bg-img"></div>

    </section>
  </div>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style scoped lang='scss'>

@import '../assets/sass/style.scss';

.footer {
  height: 300px;
  background-image: url("../assets/img/footer-bg.jpg");
}

.d-flex {
  justify-content: space-between;
}

li {

  h4 {
    margin-top: 40px;
    margin-bottom: 10px;
  }

  a {
    color: white;
  }

}

.bg-img {
  background-image: url("../assets/img/dc-logo-bg.png");
}


</style>