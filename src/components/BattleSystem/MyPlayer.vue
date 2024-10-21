<script setup>
import { ref } from 'vue';
const animationFramesPixels = ref([-411]);
</script>

<template>
    <div class="my-player">

    </div>
</template>

<style lang="scss" scoped>
    // @keyframes playerAnimation{
    //     0%{
    //         background-position-x: 0px;
    //     }
    //     100%{
    //         background-position-x: 411px;
    //     }
    // }
    @keyframes playerAnimation {
      to { background-position: -2055px; }
    }

    .my-player{
        position: absolute;
        width: 411px;
        height: 320px;
        overflow: hidden;
        background: url(../../assets/images/player/player_design.png);
        background-repeat: no-repeat;
        animation-name: playerAnimation; 
        animation-duration:2s;
        animation-timing-function: steps(5);
        animation-iteration-count: infinite;
    }
</style>