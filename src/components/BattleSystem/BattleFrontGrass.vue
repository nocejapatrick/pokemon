<script script>

</script>

<template>
    <div class="grass">

    </div>
</template>

<style lang="scss" scoped>
@keyframes grassAnimation {
    0%{
        transform: translate(0%,0%);
    }
    50%{
        transform: translate(-30%, 10%);
    }
    100%{
        transform: translate(-60%, 50%);
    }
}
.grass{
    position: absolute;
    left: -20px;    
    bottom: 190px;
    z-index: 7;
    width: 600%;
    height: 350px;
    background: url(../../assets/images/grass.png);
    background-repeat: repeat-x;
    background-size: 900px;
    animation: grassAnimation 3s linear 1s forwards;
}
</style>