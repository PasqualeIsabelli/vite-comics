<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import TheBanner from './components/TheBanner.vue';

export default {
  components: {
    TheHeader,
    TheFooter,
    TheBanner
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
        <h1 class="text-white">  Content goes here  </h1>
      </div>
    </section>
  </main>
  <TheBanner></TheBanner>

  <TheFooter></TheFooter>
</template>


<style scoped>
  .content {
    height: 180px;
    background-color: black; /*inserire tramite variabile vedere come importare sass con @use*/

    .content-box {
      margin: 0 300px;
      /* centratura verticale */
    }
  }
</style>
