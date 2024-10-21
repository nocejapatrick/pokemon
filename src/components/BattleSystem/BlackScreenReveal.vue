<script setup>

</script>

<template>
    <div class="black-screen">
        <div class="up"></div>
        <div class="down"></div>
    </div>
</template>

<style lang="scss" scoped>
@keyframes upBlackScreenReveal{
    0%{
        top:0%;
    }
    100%{
        top: -50%;
    }
}

@keyframes downBlackScreenReveal{
    0%{
        bottom:0%;
    }
    100%{
        bottom: -50%;
    }
}

.black-screen{
    position: absolute;
    top:0;
    left: 0;
    bottom: 0;
    right: 0;
    z-index: 9;

    & .up{
        position: absolute;
        top:0%;
        width: 100%;
        height: 50%;
        background: black;
        animation: upBlackScreenReveal 2s ease-in-out .5s forwards;
    }

    & .down{
        position: absolute;
        bottom: 0%;
        width: 100%;
        height: 50%;
        background: black;
        animation: downBlackScreenReveal 2s ease-in-out .5s forwards;
    }
}
</style>