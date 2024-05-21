<script setup>
import Header from "@/components/Header.vue";
import GameBoard from "@/components/GameBoard.vue";
</script>

<template>
  <div class="bg-yellow-200">
    <header>
        <Header />
    </header>
    <main>
      <div class="bg-pink-400 grid grid-cols-2 p-8 gap-8">
        <div>
          <GameBoard />
        </div>
        <div>
          <GameBoard />
        </div>
      </div>
    </main>
  </div>

</template>

<style scoped>

</style>
