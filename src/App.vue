<script setup>
import Header from "@/components/Header.vue";
import GameBoard from "@/components/GameBoard.vue";
import GameBoardCell from "@/components/GameBoardCell.vue";
</script>

<template>
  <div>
    <header>
        <Header />
    </header>
    <main>
      <div>
        <GameBoard />
      </div>
    </main>
  </div>

</template>

<style scoped>

</style>
