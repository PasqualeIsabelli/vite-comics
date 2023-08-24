<script>
export default {
  props: {
    imgSrc: String,
    title: String,
    price: Number,
    type: String,
  }
}
</script>


<template>
  <div class="card h-100 m-0 border-0">
    <img :src="imgSrc">
    <div class="card-body text-white fs-4">
      {{ title.toUpperCase() }}
    </div>
    <div class="overlay">
      <div class="fw-bold fs-1 text-center">Prezzo: {{ price }}</div>
      <div class="fw-bold fs-1 text-center">Genere: {{ type.toUpperCase() }}</div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.card {
  margin: 5rem 0 4rem 0;
  background-color: transparent;

  img {
    height: 450px;
  }
  .overlay {
    background-color: rgba(255, 255, 255, 0.5);
    position: absolute;
    inset: 0;
    opacity: 0;
    transition: opacity 0.4s ease-in-out;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    backdrop-filter: blur(5px);
  }
  &:hover{
    .overlay {
      opacity: 1;
    }
  }
}
</style>