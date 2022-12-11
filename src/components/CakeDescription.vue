<template>
  <div class="description d-flex align-ites-center">
    {{ desc }}
  </div>
</template>

<script>
export default {
  name: "CakeDescription",
  props: {
    desc: String,
  },
};
</script>

<style scoped>
.description {
  margin: 70px 70px 70px 10%;
  width: 350px;
  height: 350px;
  border-radius: 5px;
  padding: 70px 50px;

  background: rgb(255, 214, 239);
  box-shadow: rgba(0, 0, 0, 0.15) 10px 10px 2.6px;

  font-size: 1.8em;
  text-shadow: rgb(255, 170, 235) 3px 2px 1px;
  font-weight: bold;
}

@media screen and (max-width: 895px) {
  .description {
    height: 370px;
    margin: 25px 10px 0 45px;
  }
}
@media screen and (max-width: 845px) {
  .description {
    height: 350px;
    margin: 25px 10px 0 45px;
  }
}

@media screen and (max-width: 730px) {
  .description {
    height: 400px;
    margin: 25px 0 0 0;
    border-radius: 0 5px 5px 0;
  }

  @media screen and (max-width: 615px) {
    .description {
      height: 45%;
      border-radius: 5px;
    }

  }
}
</style>