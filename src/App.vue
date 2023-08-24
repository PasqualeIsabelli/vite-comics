<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import NavBar from './components/NavBar.vue';
import CardContainer from './components/CardContainer.vue';
import cardList from './assets/db/dc-comics.json';

export default {
  components: {
    TheHeader,
    TheFooter,
    NavBar,
    CardContainer
  },
  data() {
    return {
      cardList,
    }
  }
}
</script>


<template>
  <header>
    <TheHeader></TheHeader>
  </header>
  
  <main>
    <div class="bg-dark pb-5">
      <div class="jumbo-box"></div>
      <div class="series-container">
        <div class="series"><h2 class="text-white fw-bold">CURRENT SERIES</h2></div>
      </div>
      <div class="card-content row row-cols-6">
        <div class="col" v-for="(card, i) in cardList" :key="`${i}`">
          <CardContainer :img-src="card.thumb" :title="card.series"></CardContainer> <!--:price="card.price" :type="card.type"-->
        </div>
      </div>
      
      <div class="text-center">
        <button type="button" class="btn btn-primary fs-4 fw-bold rounded-0">LOAD MORE</button>
      </div>
    </div>
    <NavBar></NavBar>
  </main>

  <footer>
    <TheFooter></TheFooter>
  </footer>
</template>


<style lang="scss" scoped>
@use '../src/styles/partials/variables' as *;

.jumbo-box {
  height: 450px;
  background-image: url(../src/assets/img/jumbotron.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}
.series-container {
  margin: 0 300px;
  position: relative;
  .series {
  background-color: $color-primary;
  display: inline-block;
  padding: 1rem 1.5rem;
  position: absolute;
  top: -40px;
  }
}
.card-content {
  margin: 0 300px;
  
  button {
    margin-top: 620px; /*controllare se va bene cosi???? */
    padding: .5rem 4rem;
  }
}
</style>
