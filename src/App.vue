<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import NavBar from './components/NavBar.vue';
import Jumbo from './components/Jumbo.vue';
import Card from './assets/db/dc-comics.json';

export default {
  components: {
    TheHeader,
    TheFooter,
    NavBar,
    Jumbo
  },
  data() {
    return {
      Card,
    }
  }
}
</script>


<template>
  <header>
    <TheHeader></TheHeader>
  </header>
  
  <main>
    <Jumbo></Jumbo> <!--INSERIRE ATTR.--> 
    <NavBar></NavBar>
  </main>

  <footer>
    <TheFooter></TheFooter>
  </footer>
</template>


<style lang="scss" scoped>

</style>
