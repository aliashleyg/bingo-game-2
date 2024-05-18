<script setup>
import Header from "@/components/Header.vue";
import GameBoard from "@/components/GameBoard.vue";
</script>

<template>
  <div>

    <header>
        <Header />
    </header>

    <main>
      <div>
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
