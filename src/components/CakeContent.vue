<template>
  <div class="main d-flex">
    <img class="cake img-thumbnail m-4" :src="cake" :alt="alt" />
  </div>
</template>

<script>
export default {
  name: "CakeContent",
  props: {
    cake: String,
    alt: String,
  },
};
</script>

<style scoped>
.main {
  height: 500px;
  padding-right: 100px;
  justify-content: end;
}

.cake {
  box-shadow: rgba(0, 0, 0, 0.15) 10px 10px 2.6px;
}

@media screen and (max-width: 953px) {
  .cake {
    max-width: 350px;
    max-height: 400px;
  }
  .main {
    padding-right: 50px;
  }
}
@media screen and (max-width: 804px) {
  .cake {
    max-width: 350px;
    max-height: 350px;
  }
  .main {
    padding-right: 25px;
  }
}
@media screen and (max-width: 615px) {
  .cake {
    max-width: 320px;
    max-height: 320px;

    border-radius: 0;
  }
  .main {
    padding-right: 0;
    justify-content: center;
  }
}
</style>
