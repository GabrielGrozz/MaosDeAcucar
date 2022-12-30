<template>
    <div class="works-container">
        <div class="title-container">
            <h1 class="title fs-1 p-3 m-0">Montagem</h1>
        </div>
        <div class="subtitle-container p-4">
            <h2 class="subtitle">
                Trabalhamos com ingredientes de ótima qualidade e sempre fazendo o melhor para você 
            </h2>
        </div>
        <Montage class="cake-1" :video="cakeMontage" direction="1" />
        <Montage class="cake-2" :video="PanetoneMontage" direction="2"/>
    </div>
</template>

<script>
    import cakeMontage from "../assets/videos/montagem-bolo.mp4"
    import PanetoneMontage from "../assets/videos/montagem-panetone.mp4"

import Montage from "./Montage.vue"
    export default{
        name: "Works",
        data(){
            return{
                cakeMontage: cakeMontage,
                PanetoneMontage: PanetoneMontage
            }
        },
        components: {
            Montage
        }
    }
</script>

<style scoped>
 .title-container{
    background: rgb(255, 233, 237);
 }

 .subtitle-container{
    background: rgb(255, 154, 154);
 }

 .subtitle{
    text-shadow: white 1.5px 1.5px 0.4px;
 }

 .works-container{
    border-top: rgb(255, 115, 138) 10px solid;
    }



</style>