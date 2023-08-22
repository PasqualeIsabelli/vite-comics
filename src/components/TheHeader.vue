<script>
export default {

}
</script>


<template>
  <header class="d-flex justify-content-between">
    <img src="../assets/img/dc-logo.png" alt="dc-logo">

    <ul class="nav nav-pills d-flex justify-content-center align-items-center">
      <li class="nav-item"><a class="nav-link fw-bold" href="#">CHARACTERS</a></li>
      <li class="nav-item"><a class="nav-link fw-bold active" href="#">COMICS</a></li>
      <li class="nav-item"><a class="nav-link fw-bold" href="#">MOVIES</a></li>
      <li class="nav-item"><a class="nav-link fw-bold" href="#">TV</a></li>
      <li class="nav-item"><a class="nav-link fw-bold" href="#">GAMES</a></li>
      <li class="nav-item"><a class="nav-link fw-bold" href="#">COLLECTIBLES</a></li>
      <li class="nav-item"><a class="nav-link fw-bold" href="#">VIDEOS</a></li>
      <li class="nav-item"><a class="nav-link fw-bold" href="#">FANS</a></li>
      <li class="nav-item"><a class="nav-link fw-bold" href="#">NEWS</a></li>
      <li class="nav-item"><a class="nav-link fw-bold" href="#">SHOP</a></li>
    </ul>
  </header>
</template>


<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

header {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 18px;
  height: 180px;
  margin: 0 300px;
  padding: 25px;
  .nav-link {
    color: $black;
  }
  &.active { // da sistemare... perche non la prende?
    color: $color-primary;
    background-color: $white;
  }
}
</style>