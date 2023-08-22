<script>
export default {

}
</script>


<template>
  <main>
    <div class="main-content">
      <ul class="d-flex">
        <li class="nav-item"><img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics"><a class="nav-link text-white fs-3" href="#">DIGITAL COMICS</a></li>
        <li class="nav-item"><img src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise"><a class="nav-link text-white fs-3" href="#">DC MERCHANDISE</a></li>
        <li class="nav-item"><img src="../assets/img/buy-comics-subscriptions.png" alt="subscription"><a class="nav-link text-white fs-3" href="#">SUBSCRIPTION</a></li>
        <li class="nav-item"><img src="../assets/img/buy-comics-shop-locator.png" alt="comic shop locator"><a class="nav-link text-white fs-3" href="#">COMIC SHOP LOCATOR</a></li>
        <li class="nav-item"><img src="../assets/img/buy-dc-power-visa.svg" alt="dc power visa"><a class="nav-link text-white fs-3" href="#">DC POWER VISA</a></li>
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
    align-items: center;
  }

  img {
    width: 60px;
  }
}

</style>