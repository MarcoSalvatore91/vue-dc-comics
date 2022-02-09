<template>
  <div>
      <section v-for="(icon, index) in icons" :key="index">
          <div id="img-social">
            <img :src="require(`../assets/img/${icon.url}`)" :alt="icon.text">
          </div>
      </section>
  </div>
</template>

<script>
export default {
name: 'IconSocial',
  data() {
      return {
        icons: [
          { text: "Facebook", url: 'footer-facebook.png',},
          { text: "Periscope", url: "footer-periscope.png",},
          { text: "Pinterest", url: "footer-pinterest.png",},
          { text: "Twitter", url: "footer-twitter.png",},
          { text: "Youtube", url: "footer-youtube.png",},
        ]
      }
  }
}
</script>

<style scoped lang='scss'>
    img {
        margin-right: 10px;
    }
</style>