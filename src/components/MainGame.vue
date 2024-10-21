<script setup>
import BlackScreenReveal from './BattleSystem/BlackScreenReveal.vue';
import BattleIntercationTile from './BattleSystem/BattleInteractionTile.vue'
import BattleFrontGrass from './BattleSystem/BattleFrontGrass.vue';
import MyPlayer from './BattleSystem/MyPlayer.vue';
import { ref } from 'vue';

const revealBlackScreen = ref(false);
</script>

<template>
    <div class="main-game-container">
        <div class="main-game">
            <!-- <MyPlayer /> -->
            <BattleIntercationTile />
            <BattleFrontGrass />
            <BlackScreenReveal />
        </div>
    </div>
</template>

<style lang="scss" scoped>
.main-game-container{
    height: 100vh;
    background: #d1d1d1;
    width: 700px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.main-game{
    width: 100%;
    height: 600px;
    position: relative;
    overflow: hidden;
    background: gray;
}
</style>