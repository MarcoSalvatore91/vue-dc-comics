<template>
  <div class="main">

    <!-- Contents -->
    <section class="contents">
      <div class="container d-flex">
        <Card v-for="(serie, index) in series" :key="index"
        :serie="serie"
        />
        <div class="btn">
          <button class="color-white">LOAD MORE</button>
        </div>
      </div>
    </section>

  </div>
</template>

<script>
import Card from './Card.vue'

export default {
    name: 'Main',
    components: {
      Card,
    },
    props: ["series"],
}
</script>

<style scoped lang='scss'>

@import '../assets/sass/style.scss';

.contents {
  background-color: black;
  min-height: 700px;
  position: relative;

  .d-flex {
    flex-wrap: wrap; 
  }

    .btn button {
      position: absolute;
      left: 40%;
      bottom: 30px;
      padding: 10px 40px;
      background-color: rgb(2,130,249);
      font-weight: bold;
    }
}



</style>