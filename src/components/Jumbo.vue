<script>
export default {
  props: {
    imgSrc: String,
    // INSERIRE GLI ALTRI PROPS
  }
}
</script>


<template>
  <div class="content bg-dark">
    <div class="jumbo-box"></div>
    <div class="jumbo-content">
      <div class="series"><h2 class="text-white fw-bold">CURRENT SERIES</h2></div>
    </div>

    <div class="card-container">
      <div class="card">
        <img :src="imgSrc"> <!--DA SISTEMARE-->
        <div class="card-body">
          {{  }} <!--INSERIRE QUI IL TITOLO (SERIES) INSIEME AL .toUpperCase() PER RENDERE LE TUTTE LE LETTERE MAIUSCOLE-->
        </div>
        <div class="overlay">
          <span> <!-- INSERIRE QUI IL PREZZO (PRICE)--> </span>
          <span> <!-- INSERIRE QUI IL TIPO (TYPE)--> </span>
        </div>
      </div>

      <div class="text-center">
        <button type="button" class="btn btn-primary fs-4 fw-bold rounded-0">LOAD MORE</button>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.content {
  height: 1200px;
  .jumbo-box {
    height: 450px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
  }
  .jumbo-content {
    margin: 0 300px;
    position: relative;
    .series {
      background-color: $color-primary;
      display: inline-block;
      padding: 1rem 1.5rem;
      position: absolute;
      top: -40px;
    }
    button {
      margin-top: 620px; /*controllare se va bene cosi???? */
      padding: .5rem 4rem;
    }
  }

  .card-container {
    margin: 0 300px;
    .card {
    margin: 5rem 0 4rem 0;
    // background-color: transparent;
    }
  } 
}
</style>