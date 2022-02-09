<template>
  <div>
    <img :src="serie.thumb" :alt="serie.type"> 
    <figcaption class="color-white">{{ serie.series }}</figcaption>
  </div>
</template>

<script>
export default {
    name: 'Card',
    props: ["serie"],
}
</script>

<style scoped lang='scss'>

@import '../assets/sass/style.scss';

    img {
      width: 150px;
      height: 200px;
      margin: 40px 20px 0 20px;
    }

    figcaption {
      margin: 10px 20px 20px 20px;
      width: 150px;
    }

</style>