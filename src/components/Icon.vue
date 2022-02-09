<template>
  <div>
    <section id="info">
      <div class="container d-flex">
        <div class="d-flex" v-for="(link, index) in links" :key="index">
          <div class="sec-img">
            <img :src="require(`../assets/img/${link.url}`)" alt="">
          </div>
          <div>
            <span class="color-white">{{ link.text }}</span>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Icon',
  data() {
      return {
        links: [
          { text: "DIGITAL COMICS", url: 'buy-comics-digital-comics.png',},
          { text: "DC MERCHANDISE", url: "buy-comics-merchandise.png",},
          { text: "SUBSCRIPTION", url: "buy-comics-subscriptions.png",},
          { text: "COMIC SHOP LOCATOR", url: "buy-comics-shop-locator.png",},
          { text: "DC POWER VISA", url: "buy-dc-power-visa.svg",},
        ]
      }
  }
}
</script>

<style scoped lang='scss'>

  #info {
  background-color: rgb(2,130,249);
  height: 160px;

    .d-flex {
      justify-content: space-evenly;
    }

    .sec-img {
      line-height: calc(160px + 50px);

      img {
        height: 50px;
      }
    }


    span {
      font-size: 0.8rem;
      margin: 0 30px 0 10px;
      line-height: 180px;
    }
  }


</style>