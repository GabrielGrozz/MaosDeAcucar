<template>
  <div>
    <Header class="header d-flex justify-content-center" />
    <Main />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
  },
};
</script>

<style scoped>
.header {
  height: 40vh;
}
</style>