<script setup>
  import { ref } from "vue"

  const header = ref("B")
  const items = ref([
    {id: 1, label: "Value 1"},
    {id: 2, label: "Value 2"},
    {id: 3, label: "Value 3"},
    {id: 4, label: "Value 4"},
    {id: 5, label: "Value 5"},
  ])
  const addToList = ref("")
  const howImportantIsThis =ref(false)
</script>

<template>
  <h1>{{ header }}</h1>
  <form
      v-on:submit.prevent="items.push({id:items.length + 1, label: addToList})">
    <input v-model=addToList
           type="text"
           placeholder= "Let's add something to our list!"
    />
    Priority:
    <label>
      <input type="checkbox"
             v-model="howImportantIsThis" />
      High Priority
    </label>
    <button class="bg-yellow-200 text-red-600 rounded-full px-4">
      Add!
    </button>
  </form>
  <ul>
    <li v-for="({id, label}, index) in items" :key="id">
      {{ index }}
      {{ label }}</li>
  </ul>

</template>

<style scoped>

</style>