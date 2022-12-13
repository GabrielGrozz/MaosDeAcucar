<template>
    <div :class="'montage'+ direction">
        <div class="montage-video">
            <video controls controlslist="video-content nofullscreen nodownload noremoteplayback noplaybackrate foobar" width="250" >
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
            video: String,
            direction: String

        }

    }
</script>

<style scoped>

    .montage1{
        display: flex;
        padding: 50px 150px;
        background: rgb(255, 188, 197);
    }
    .montage2{
        display: flex;
        flex-direction: row-reverse;
        padding: 25px 150px;
        background: rgb(255, 188, 197);
    }

    .montage-video{
        border: 5px rgb(255, 255, 255) solid;
        border-radius: 5px;
        box-shadow: rgb(239, 145, 232) 7px 7px 3px;
    }
</style>