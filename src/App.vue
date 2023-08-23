<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import NavBar from './components/NavBar.vue';
import Jumbo from './components/Jumbo.vue'

export default {
  components: {
    TheHeader,
    TheFooter,
    NavBar,
    Jumbo
  },
  data() {
    return {}
  }
}
</script>


<template>
  <header>
    <TheHeader></TheHeader>
  </header>
  
  <main>
    <Jumbo></Jumbo>
    <NavBar></NavBar>
  </main>

  <footer>
    <TheFooter></TheFooter>
  </footer>
</template>


<style lang="scss" scoped>

</style>
