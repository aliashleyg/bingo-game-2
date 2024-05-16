<script setup>
 let columnNumbers = []
 let low;
 let high;
 let total;
function generateRandomInt(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

function generateColumnData(low, high, total) {
  total = 5;
  for (let i = 1; i <= total; i++) {
    let unfiledValue = (generateRandomInt(1,15));
    if (!columnNumbers.includes(unfiledValue)) {
      columnNumbers.push(unfiledValue);
      console.log(i + " " + unfiledValue);
    } else {
      i--;
      console.log(i + " duplicate of " + unfiledValue);
    }
  }
  return columnNumbers;
}

</script>

<template>
  <div class="grid grid-cols-1 gap-x-4 gap-y-4 md:gap-x-8">
    <div v-html="generateColumnData(1, 15, 5)">
</div>
  </div>

</template>

<style scoped>

</style>