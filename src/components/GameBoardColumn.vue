<!--  <script setup>-->
<!--  let columnNumbers = []-->

<!--  const row1params = {-->
<!--    low: 1, high: 15-->
<!--  }-->
<!--  const row2params = {-->
<!--    low: 16, high: 30-->
<!--  }-->
<!--  const row3params = {-->
<!--    low: 31, high: 45-->
<!--  }-->
<!--  const row4params = {-->
<!--    low: 46, high: 60-->
<!--  }-->
<!--  const row5params = {-->
<!--    low: 61, high: 75-->
<!--  }-->
<!--const cellToHide = columnNumbers[12];-->

<!--  function generateRandomInt(min, max) {-->
<!--    return Math.floor(Math.random() * (max - min + 1)) + min;-->
<!--  }-->

<!--  function generateColumnData(low, high) {-->
<!--    let total = 5;-->
<!--    for (let i = 1; i <= total; i++) {-->
<!--      let unfiledValue = (generateRandomInt(low, high));-->
<!--      if (!columnNumbers.includes(unfiledValue)) {-->
<!--        columnNumbers.push(unfiledValue);-->
<!--      } else {-->
<!--        i&#45;&#45;;-->
<!--      }-->
<!--    }-->
<!--    return columnNumbers;-->
<!--  }-->

<!--  generateColumnData(row1params.low, row1params.high);-->
<!--  generateColumnData(row2params.low, row2params.high);-->
<!--  generateColumnData(row3params.low, row3params.high);-->
<!--  generateColumnData(row4params.low, row4params.high);-->
<!--  generateColumnData(row5params.low, row5params.high);-->

<!--  let columnB = columnNumbers.slice(0, 5);-->
<!--  let columnI = columnNumbers.slice(5, 10);-->
<!--  let columnN = columnNumbers.slice(10, 15);-->
<!--  let columnG = columnNumbers.slice(15, 20);-->
<!--  let columnO = columnNumbers.slice(20, 25);-->
<!--  </script>-->

<!--  <template>-->
<!--    <div class="bg-green-800 grid grid-cols-5 border-amber-100 border-2 border-solid">-->
<!--      <div ref class="bg-blue-800">-->
<!--        <li class="grid grid-rows-1 h-40" v-for="cellNumber in columnB">-->
<!--          {{ cellNumber }}-->
<!--        </li>-->
<!--      </div>-->
<!--      <div>-->
<!--        <li class="grid grid-rows-1 h-40" v-for="cellNumber in columnI">-->
<!--          {{ cellNumber }}-->
<!--        </li>-->
<!--      </div>-->
<!--      <div>-->
<!--        <li class="grid grid-rows-1 h-40"  v-for="cellNumber in columnN">-->
<!--          {{ cellNumber }}-->
<!--        </li>-->
<!--      </div>-->
<!--      <div>-->
<!--        <li class="grid grid-rows-1 h-40" v-for="cellNumber in columnG">-->
<!--          {{ cellNumber }}-->
<!--        </li>-->
<!--      </div>-->
<!--      <div>-->
<!--        <li class="grid grid-rows-1 h-40" v-for="cellNumber in columnO">-->
<!--          {{ cellNumber }}-->
<!--        </li>-->
<!--      </div>-->
<!--  </div>-->

<!--  </template>-->

<!--  <style scoped>-->
<!--.hide {-->
<!--  visibility: hidden;-->
<!--}-->
<!--  </style>-->