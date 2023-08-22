<script>
export default {

}
</script>


<template>
  <footer>
    <section class="up d-flex">
      <div class="d-flex justify-content-between footer-box-up">
        <div class="ul-container d-flex">
          <div>
            <ul>
              <h3 class="text-white fw-bold">DC COMICS</h3>
              <li class="nav-item"><a class="nav-link" href="#">Characters</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Comics</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Movies</a></li>
              <li class="nav-item"><a class="nav-link" href="#">TV</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Games</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Videos</a></li>
              <li class="nav-item"><a class="nav-link" href="#">News</a></li>
            </ul>
            <ul>
              <h3 class="text-white fw-bold pt-5">SHOP</h3>
              <li class="nav-item"><a class="nav-link" href="#">Shop DC</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="ms-3">
            <ul>
              <h3 class="text-white fw-bold">DC</h3>
              <li class="nav-item"><a class="nav-link" href="#">Terms Of Use</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Privacy policy (New)</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Ad Choices</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Advertising</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Jobs</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Subscriptions</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Talent Workshops</a></li>
              <li class="nav-item"><a class="nav-link" href="#">CPSC Certificates</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Ratings</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Shop Help</a></li>
              <li class="nav-item"><a class="nav-link" href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="ms-3">
            <ul>
              <h3 class="text-white fw-bold">SITES</h3>
              <li class="nav-item"><a class="nav-link" href="#">DC</a></li>
              <li class="nav-item"><a class="nav-link" href="#">MAD Magazine</a></li>
              <li class="nav-item"><a class="nav-link" href="#">DC Kids</a></li>
              <li class="nav-item"><a class="nav-link" href="#">DC Universe</a></li>
              <li class="nav-item"><a class="nav-link" href="#">DC Power Visa</a></li>
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
          <img src="../assets/img/footer-facebook.png" alt="facebook">
          <img src="../assets/img/footer-twitter.png" alt="twitter">
          <img src="../assets/img/footer-youtube.png" alt="youtube">
          <img src="../assets/img/footer-pinterest.png" alt="pinterest">
          <img src="../assets/img/footer-periscope.png" alt="periscope">
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
}</style>