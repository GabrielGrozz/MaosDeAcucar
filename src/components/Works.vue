<template>
    <div class="works-container">
        <div class="title-container">
            <h1 class="title fs-1 p-3">Montagem</h1>
        </div>
        <div class="subtitle">
            <h2>
                Trabalhamos com ingredientes de ótima qualidade e sempre fazendo o melhor para você 
            </h2>
        </div>
        <Montage :video="cakeMontage" />
        <Montage :video="PanetoneMontage" />
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

 .works-container{
    border-top: rgb(255, 115, 138) 10px solid
    }

</style>