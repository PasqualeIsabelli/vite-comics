<script>
export default {
  data() {
    return {
      creditsList: [
        {
          title: 'DC COMICS',
          credits: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"]
        },
        {
          title: 'SHOP',
          credits: ["Shop DC", "Shop DC Collectibles"]
        },
        {
          title: 'DC',
          credits: ["Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"]
        },
        {
          title: 'SITES',
          credits: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]
        }
      ]
    }
  }
}
</script>


<template>
  <footer>
    <section class="up d-flex">
      <div class="d-flex justify-content-between footer-box-up">
        <div class="ul-container d-flex">
          <div class="d-flex flex-column flex-wrap">
            <ul v-for="singleCredit in creditsList">
              <h3 class="text-white fw-bold"> {{ singleCredit.title }}</h3>
              <li v-for="singleLink in singleCredit.credits" class="nav-item list-unstyled"><a class="nav-link" href="#">{{ singleLink }}</a></li>
            </ul>
          </div>
        </div>
        <div class="dc-bg"></div>
      </div>
    </section>

    <section class="down">
      <div class="d-flex justify-content-between footer-box-down">
        <div class="footer-down-content">
          <button type="button" class="btn btn-outline-primary text-white fs-3 fw-bold p-3">SIGN-UP NOW!</button>
        </div>
        <div class="footer-down-content d-flex gap-5">
          <a href="#" class="fs-3 fw-bold text-primary">FOLLOW US</a>
          <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
          <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
          <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
          <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
          <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
        </div>
      </div>
    </section>
  </footer>
</template>


<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

footer {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 18px;

  .up {
    height: 600px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    .footer-box-up {
      width: 100%;
      margin: 0 300px;

      .ul-container {
        padding: 50px 25px;
      }

      .dc-bg {
        height: 100%;
        width: 900px;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: 0px;
      }
    }
  }

  h3 {
    padding-bottom: 1rem;
  }

  .nav-link {
    color: $color-text;
  }

  .down {
    background-color: $color-secondary;
    height: 150px;

    .footer-box-down {
      margin: 0 300px;
      height: 100%;
    }

    .footer-down-content {
      display: flex;
      align-items: center;

      .text-primary {
        color: $color-primary;
        text-decoration: none;
      }

      img {
        width: 60px;
      }
    }
  }
}
</style>