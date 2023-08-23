<script>
export default {
  data() {
    return {
      iconList: [
        {
          title: 'DIGITAL COMICS',
          img: '../assets/img/buy-comics-digital-comics.png'
        },
        {
          title: 'DC MERCHANDISE',
          img: '../assets/img/buy-comics-merchandise.png'
        },
        {
          title: 'SUBSCRIPTION',
          img: '../assets/img/buy-comics-subscriptions.png'
        },
        {
          title: 'COMIC SHOP LOCATOR',
          img: '../assets/img/buy-comics-shop-locator.png'
        },
        {
          title: 'DC POWER VISA',
          img: '../assets/img/buy-dc-power-visa.svg'
        }
      ]
    }
  },
  methods: {
    getSingleImage(singleImage) {
      new URL(`${singleImage}`, import.meta.url).href 
    }
  }
}
</script>


<template>
  <main>
    <div class="main-content">
      <ul class="d-flex list-unstyled">
        <li class="nav-item" v-for="singleIcon in iconList"><a class="nav-link text-white fs-3" href="#"><img :src="getSingleImage(singleIcon.img)"> {{ singleIcon.title }}</a></li> <!--sistemare-->
      </ul>
    </div>
  </main>
</template>


<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

main {
  background-color: $color-primary;
  height: 220px;

  .main-content {
    margin: 0 300px;
  }

  ul {
    justify-content: space-between;
    /*centratura verticale*/
  }

  img {
    width: 70px;
  }
}</style>