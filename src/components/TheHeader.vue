<script>
export default {
  data() {
    return {
      menuList: [
        {
          name: 'CHARACTERS'
        },
        {
          name: 'COMICS'
        },
        {
          name: 'MOVIES'
        },
        {
          name: 'TV'
        },
        {
          name: 'GAMES'
        },
        {
          name: 'COLLECTIBLES'
        },
        {
          name: 'VIDEOS'
        },
        {
          name: 'FANS'
        },
        {
          name: 'NEWS'
        },
        {
          name: 'SHOP'
        }
      ]
    }
  }
}
</script>


<template>
  <header class="d-flex justify-content-between">
    <img src="../assets/img/dc-logo.png" alt="dc-logo">

    <ul class="nav nav-pills d-flex justify-content-center align-items-center">
      <li v-for="singleItem in menuList" class="nav-item"><a class="nav-link fw-bold" href="#"> {{ singleItem.name }}</a></li>
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

  &.active {
    // da sistemare... perche non la prende?
    color: $color-primary;
    background-color: $white;
  }
}</style>