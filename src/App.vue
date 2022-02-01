<template>
  <ol>
    <li v-for="(student, index) in students" :key="student.id">Index - [{{ index }}] {{ student.name }}</li>
  </ol>
</template>

<script>
export default {
  data() {
    return {
      students: [
        {id: 1, name: "Andre"},
        {id: 2, name: "Matiew"},
        {id: 3, name: "Leonel"},
      ]
    }
  }
}
</script>

<style>

</style>