  <script setup>
  let columnNumbers = []

  const row1params = {
    low: 1, high: 15, total: 5
  }
  const row2params = {
    low: 16, high: 30, total: 5
  }
  const row3params = {
    low: 31, high: 45, total: 4
  }
  const row4params = {
    low: 46, high: 60, total: 5
  }
  const row5params = {
    low: 61, high: 75, total: 5
  }

  function generateRandomInt(min, max) {
    return Math.floor(Math.random() * (max - min + 1)) + min;
  }

  function generateColumnData(low, high, total) {
    for (let i = 1; i <= total; i++) {
      let unfiledValue = (generateRandomInt(low, high));
      if (!columnNumbers.includes(unfiledValue)) {
        columnNumbers.push(unfiledValue);
      } else {
        i--;
      }
    }
    return columnNumbers;
  }

  generateColumnData(row1params.low, row1params.high, row1params.total);
  generateColumnData(row2params.low, row2params.high, row2params.total);
  generateColumnData(row3params.low, row3params.high, row3params.total);
  generateColumnData(row4params.low, row4params.high, row4params.total);
  generateColumnData(row5params.low, row5params.high, row5params.total);

  let columnB = columnNumbers.slice(0, 5);
  let columnI = columnNumbers.slice(5, 10);
  let columnN = columnNumbers.slice(10, 14);
  let columnG = columnNumbers.slice(14, 19);
  let columnO = columnNumbers.slice(19, 25);
  </script>

  <template>
    <div>

      <div>
        <li v-for="cellNumber in columnB">
          {{ cellNumber }}
        </li>
      </div>
      <div>
        <li v-for="cellNumber in columnI">
          {{ cellNumber }}
        </li>
      </div>
      <div>
        <li v-for="cellNumber in columnN">
          {{ cellNumber }}
        </li>
      </div>
      <div>
        <li v-for="cellNumber in columnG">
          {{ cellNumber }}
        </li>
      </div>
      <div>
        <li v-for="cellNumber in columnO">
          {{ cellNumber }}
        </li>
      </div>
  </div>

  </template>

  <style scoped>

  </style>