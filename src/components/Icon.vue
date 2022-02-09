<template>
  <div>
      <section id="info">
      <div v-for="link in links" :key="link.text">
        <img :src="`../assets/img/${link.url}`" alt="">
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
          { text: "DC MERCHANDISE", url: "buy-comics-digital-merchandise.png",},
          { text: "SUBSCRIPTION", url: "buy-comics-subscriptions.png",},
          { text: "COMIC SHOP LOCATOR", url: "buy-comics-shop-locator.png",},
          { text: "DC POWER VISA", url: "buy-dc-power-visa.svg",},
        ]
      }
    }
}
</script>

<style>

  #info {
  background-color: rgb(2,130,249);
  height: 160px;
  }

</style>