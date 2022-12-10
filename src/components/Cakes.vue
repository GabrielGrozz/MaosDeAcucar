<template>
  <div class="conatainer-fluid">
    <div :class="['container-fluid p-0', 'bg-color-' + color]">
      <CakeName
        ><h2 class="cake-name">{{ name }}</h2></CakeName
      >
      <div class="cakes-container">
        <CakeDescription class="cake-desc" :desc="description" />
        <CakeContent :cake="cake" :alt="name" :class="'bg-color-' + color" />
      </div>
    </div>
  </div>
</template>

<script>
import CakeName from "./CakeName.vue";
import CakeContent from "./CakeContent.vue";
import CakeDescription from "./CakeDescription.vue";

export default {
  name: "Cakes",
  data() {
    return {};
  },
  components: {
    CakeName,
    CakeContent,
    CakeDescription,
  },
  props: {
    cake: String,
    name: String,
    color: String,
    description: String,
  },
}
</script>

<style scoped>
.container-fluid {
  border-top: rgb(255, 115, 138) 10px solid;
}

.cake-name {
  font-size: 2.5em;
  text-shadow: rgba(135, 135, 135, 0.4) 3px 2px 1px;
}

.cakes-container {
  display: flex;
  justify-content: space-between;
}
</style>