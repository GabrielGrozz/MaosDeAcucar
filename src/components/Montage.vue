<template>
    <div class="montage p-3">
        <div class="montage-video">
            <video controls controlslist="nofullscreen nodownload noremoteplayback noplaybackrate foobar" width="250" >
                <source :src="video" type="video/mp4">
            </video>
        </div>
    </div>
</template>

<script>
    export default{
        name: "Montage",
        data(){
            return{

            }
        },
        props: {
            video: String
        }

    }
</script>

<style scoped>

    .montage{
        display: flex;
    }
</style>