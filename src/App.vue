<script setup>
import Header from "@/components/Header.vue";
import GameBoard from "@/components/GameBoard.vue";
</script>

<template>
  <div class="container grid">

    <header>
      <div class="grid grid-cols-5">
        <Header />
      </div>
    </header>

    <main>
      <div class="grid grid-cols-5 grid-rows-5 border-2">
        <GameBoard />
      </div>
    </main>
  </div>

</template>

<style scoped>
</style>
