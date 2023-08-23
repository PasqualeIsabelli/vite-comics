<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import NavBar from './components/NavBar.vue';

export default {
  components: {
    TheHeader,
    TheFooter,
    NavBar
  },
  data() {
    return {}
  }
}
</script>

<template>
  <TheHeader></TheHeader>

  <main>
    <section class="content bg-dark">
      <div class="content-box">
        <h1 class="text-white">Content goes here</h1>
      </div>
    </section>

    <NavBar></NavBar>
  </main>

  <TheFooter></TheFooter>
</template>

<style lang="scss" scoped>
@use "./styles/partials/variables" as *;

.content {
  height: 180px;
  background-color: $black;

  .content-box {
    margin: 0 300px;
    /*centratura verticale */
  }
}
</style>
