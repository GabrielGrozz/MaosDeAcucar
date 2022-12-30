<template>
  <div class="main-app">
    <Header class="header d-flex justify-content-center" />
    <Main class="main"/>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue"

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer
  },
};
</script>

<style scoped>
.header {
  height: 40vh;
}
.main-app{
  background: rgb(255, 160, 176);
}
.main{
  border: rgba(255, 0, 102,0.5) solid 3px;
  border-bottom: 0;
}
</style>