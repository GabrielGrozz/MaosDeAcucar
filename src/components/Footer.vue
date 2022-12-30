<template><div class="footer">
    <div>
        <p class="text">
            Developed with <img :src="heart" alt="love">
        </p>
    </div>
</div></template>

<script>
import heart from "../assets/imgs/heart-icon.png"
export default {
  name: "Footer",
  data(){
    return{
        heart: heart
    }
  }
};
</script>

<style scoped>
.footer{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 150px;
    background: rgb(0, 0, 0);
}

.text{
    font-family: Arial, Helvetica, sans-serif;
    color: white;
}

</style>