<template>
  <div>
      <section id="info">
      <div v-for="link in links" :key="link.text">
        <img :src="link.src" alt="">
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
          { text: "DIGITAL COMICS", src: '../assets/img/buy-comics-digital-comics.png',},
          { text: "DC MERCHANDISE", src: "../assets/img/buy-comics-digital-merchandise.png",},
          { text: "SUBSCRIPTION", src: "../assets/img/buy-comics-subscriptions.png",},
          { text: "COMIC SHOP LOCATOR", src: "../assets/img/buy-comics-shop-locator.png",},
          { text: "DC POWER VISA", src: "../assets/img/buy-dc-power-visa.svg",},
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