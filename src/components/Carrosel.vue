<template>
  <div class="container-fluid p-5">

    <h2 class="mb-4">Alguns de nossos bolos</h2>
    <div
      id="carouselExampleControls"
      class="carousel slide"
      data-bs-ride="carousel"
    >
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img
            :src="boloBrigadeiro"
            class="d-block w-50"
            alt="bolo de brigadeiro..."
          />
        </div>
        <div class="carousel-item">
          <img
            :src="boloBrownie"
            class="d-block w-50"
            alt="bolo de brownie com morango..."
          />
        </div>
        <div class="carousel-item">
          <img
            :src="boloQuatroLeites"
            class="d-block w-50"
            alt="bolo quatro leites..."
          />
        </div>
        <div class="carousel-item">
          <img
            :src="boloBrigadeiroEninho"
            class="d-block w-50"
            alt="bolo brigadeiro com ninho..."
          />
        </div>
      </div>
      <button
        class="carousel-control-prev"
        type="button"
        data-bs-target="#carouselExampleControls"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        data-bs-target="#carouselExampleControls"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  </div>
</template>

<script>
import boloBrigadeiro from "../assets/imgs/cakes/bolo1.jpg";
import boloBrownie from "../assets/imgs/cakes/bolo2.jpg";
import boloBrigadeiroEninho from "../assets/imgs/cakes/bolo3.jpg";
import boloQuatroLeites from "../assets/imgs/cakes/bolo4.jpg";

export default {
  name: "Carrosel",
  data() {
    return {
      boloBrigadeiro: boloBrigadeiro,
      boloBrownie: boloBrownie,
      boloBrigadeiroEninho: boloBrigadeiroEninho,
      boloQuatroLeites: boloQuatroLeites,
    };
  },
};
</script>

<style scoped>
.carousel {
  background: red;
}

.carousel-inner{
    height: 100%;
}

.carousel-item {
  padding-left: 33%;
  background: rgb(255, 185, 197);
}
.container-fluid {
  background: rgb(255, 210, 241);
}

@media screen and (max-width: 820px) {
    .carousel-item {
        background: rgb(168, 79, 94);
    }
    img{
        height: 100%
    }
}
</style>