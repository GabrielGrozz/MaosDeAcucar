<template>
  <div class="main-container">
    <div class="description p-5">
      <p class="fs-1 fw-semibold">
        Bolos, doces e quiches gourmets feitos com amor
      </p>
    </div>
    <div class="context">
      <h2 class="fs-1 p-3 m-0">Alguns de nossos trabalhos</h2>
    </div>
    <div>
      <Cakes
        :cake="boloBrigadeiro"
        name="Brigadeiro"
        color="1"
        :description="descBoloBrigadeiro"
      />
      <Cakes
        :cake="boloBrownie"
        name="Brownie com Mirtilos"
        color="2"
        :description="descBoloBrownie"
      />
      <Cakes
        :cake="boloBrigadeiroEninho"
        name="Brigadeiro com Ninho"
        color="3"
        :description="descBoloNinho"
      />
      <Cakes
        :cake="boloQuatroLeites"
        name="Quatro leites"
        color="4"
        :description="descBoloQuatroLeites"
      />
    </div>
    <Works />
  </div>
</template>

<script>
import Cakes from "./Cakes.vue";
import Works from "./Works.vue";

import boloBrigadeiro from "../assets/imgs/cakes/bolo1.jpg";
import boloBrownie from "../assets/imgs/cakes/bolo2.jpg";
import boloBrigadeiroEninho from "../assets/imgs/cakes/bolo3.jpg";
import boloQuatroLeites from "../assets/imgs/cakes/bolo4.jpg";
export default {
  name: "Main",
  data() {
    return {
      boloBrigadeiro: boloBrigadeiro,
      boloBrownie: boloBrownie,
      boloBrigadeiroEninho: boloBrigadeiroEninho,
      boloQuatroLeites: boloQuatroLeites,

      descBoloBrigadeiro:
        "Um bolo de brigadeiro extremamente recheado com chocolate",
      descBoloBrownie:
        "Um bolo de brownie de café com muitos morangos e mirtilos",
      descBoloNinho:
        "Um delicioso bolo de brownie com muito brigadeiro de ninho e nutella",
      descBoloQuatroLeites:
        "Um belo Naked Cake de Quatro leites com geleia de frutas vermelhas",
    };
  },
  components: {
    Cakes,
    Works,
  },
};
</script>

<style scoped>
.main-container {
  margin: 0 auto;
  max-width: 992px;
  background: rgb(255, 197, 207);
}

.description {
  box-shadow: inset 0 1px 15px rgb(56, 56, 56);
}

.context {
  background: rgb(255, 233, 237);
}
</style>