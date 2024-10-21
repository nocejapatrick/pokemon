<script setup>

</script>

<template>
    <div class="tile">
        <div class="inner-tile">

        </div>
    </div>
</template>

<style lang="scss" scoped>
.tile{
    position: absolute;
    bottom: 0px;
    border: 5px solid #aa984a;
    width: 100%;
    height: 30%;
    z-index: 8;
    & .inner-tile{
        width: 100%;
        height: 100%;
        border: 5px solid #bcb5bb;
        background-color: #274555;
    }
}
</style>