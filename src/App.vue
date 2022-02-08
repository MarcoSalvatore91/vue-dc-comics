<template>
  <div>
    <section class="bg-dark h-100">
      <div>
        <Header />
        <Main />
        <Footer />
      </div>
    </section>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<style lang='scss'>

@import './assets/sass/style.scss';
  
</style>
