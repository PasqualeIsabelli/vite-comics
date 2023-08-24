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
  <div class="card border-0 h-100">
    <img :src="imgSrc">
    <div class="card-body text-white fs-4">
      {{ title.toUpperCase() }}
    </div>
    <div class="overlay">
      <span>Prezzo: {{ price }}</span>
      <span>Genere: {{ type }}</span>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.card {
  margin: 5rem 0 4rem 0;
  background-color: transparent;
  height: 100px;
  .overlay {
    background-color: rgba(255, 255, 255, 0.5);
    opacity: 0;
  }
  &.hover{
    .overlay {
      opacity: 1;
    }
  }
}
</style>