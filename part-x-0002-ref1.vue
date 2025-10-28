<script setup>

  import {ref} from "vue"

  let year = ref(2025)

  function yearUp() {
    year.value++
  }

</script>

<template>
  
  <p>Year is {{ year }} </p>

  <button @click="yearUp">Year ++</button>
  
</template>

<style scoped>

</style>
