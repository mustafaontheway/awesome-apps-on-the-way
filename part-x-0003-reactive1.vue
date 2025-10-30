<script setup>

  import {reactive} from "vue"

  const empData = reactive({
    "name": "Ayhan Bilir",
    "dep": "Marketing",
    "salary": 42_000
  })

  function salaryChange() {
    empData.salary += 5000
  }

</script>

<template>
  
  <div>
    Employee name: {{ empData.name }} - department: {{ empData.dep }} - salary: {{ empData.salary }} ₺
  </div>

  <button @click="salaryChange">Salary Increase (5000 ₺)</button>
  
</template>

<style scoped>

</style>
