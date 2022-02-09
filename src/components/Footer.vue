<template>
  <div>

    <div class="bg-footer">

      <section class="d-flex container">

        <div>
          <ul>
            <li><h4>DC COMICS</h4></li>
            <li v-for="comic in comics" :key="comic.text">
              <a :href="comic.url">{{ comic.text }}</a>
            </li>
          </ul>
          <ul>
            <li><h4>SHOP</h4></li>
            <li v-for="shop in shops" :key="shop.text">
              <a :href="shop.url">{{ shop.text }}</a>
            </li>
          </ul>
        </div>

        <div>
          <ul>
            <li><h4>DC</h4></li>
            <li v-for="dc in dc" :key="dc.text">
              <a :href="dc.url">{{ dc.text }}</a>
            </li>
          </ul>
        </div>

        <div>
          <ul>
            <li><h4>SITES</h4></li>
            <li v-for="site in sites" :key="site.text">
              <a :href="site.url">{{ site.text }}</a>
            </li>
          </ul>
        </div>

        <div class="bg-img"></div>

      </section>

    </div>

    <section id="foot">

      <div class="d-flex container">

        <div id="sign-up">
          <button><span>SIGN-UP NOW</span></button>
        </div>

        <div id="social" class="d-flex">
          <div>
            <h3>FOLLOW US</h3>
          </div>
          <div>
            <IconFooter class="d-flex" />
          </div>
        </div>

      </div>

    </section>

  </div>
</template>

<script>
import IconFooter from "./IconFooter.vue"

export default {
    name: 'Footer',
    components: {
      IconFooter,
    },
    data() {
    return {

      comics: [
        { text: "Characters", url: "#",},
        { text: "Comics", url: "#",},
        { text: "Movies", url: "#",},
        { text: "TV", url: "#",},
        { text: "Games", url: "#",},
        { text: "Videos", url: "#",},
        { text: "News", url: "#",},
      ],

      shops: [
        {text: "Shop DC", url: "#",},
        {text: "Shop DC Collectibles", url: "#",},
      ],

      dc: [
        { text: "Terms of Use", url: "#",},
        { text: "Privacy policy (New)", url: "#",},
        { text: "Ad choices", url: "#",},
        { text: "Advertising", url: "#",},
        { text: "Jobs", url: "#",},
        { text: "Subscriptions", url: "#",},
        { text: "Talent Workshops", url: "#",},
        { text: "CPSC Certificates", url: "#",},
        { text: "Ratings", url: "#",},
        { text: "Shop Help", url: "#",},
        { text: "Contact Us", url: "#",},
      ],

      sites: [
        { text: "DC", url: "#",},
        { text: "MAD Magazine", url: "#",},
        { text: "DC Kids", url: "#",},
        { text: "DC Universe", url: "#",},
        { text: "DC Power Visa", url: "#",},
      ],

      img: [
        {  }
      ]

    }
  }
}
</script>

<style scoped lang='scss'>

@import '../assets/sass/style.scss';

.bg-footer {
  height: 350px;
  background-image: url("../assets/img/dc-logo-bg.png"), url("../assets/img/footer-bg.jpg");
  background-size: 400px, 100%;
  background-position: 75% 70%;
  background-size: 500px, 100%; 
  background-repeat: no-repeat, no-repeat;
}

h4 {
  margin-top: 40px;
  margin-bottom: 10px;
  color: white;
}

li {

  a {
    color: grey;
  }

}

#foot {
  background-color: rgb(48,48,48);
  height: 100px;

  .d-flex {
    justify-content: space-between;
    align-items: center;
  }

  #sign-up {
    line-height: 100px;

    button {
      background-color: rgb(48,48,48);
      border: 2px solid blue;
      padding: 10px;

      span {
        color: white;
      }

    }

  }
  
}

#social {
  h3 {
    color: rgb(2,130,249);
    margin-right: 20px;
  }
}


</style>