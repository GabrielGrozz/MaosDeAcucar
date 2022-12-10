<template>
  <div class="header-container d-flex pt-4">
    <img class="logo" :src="logo" alt="logo" />
  </div>
</template>

<script>
import logo from "../assets/imgs/logo/logo.png";

export default {
  name: "Header",
  data() {
    return {
      logo: logo,
    };
  },
};
</script>

<style scoped>
.header-container {
  background: rgb(255, 160, 176);
}

.logo {
  height: 70%;
}
</style>