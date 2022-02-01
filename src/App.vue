<template>
  <div :class="status ? 'success' : 'failed'">Status</div>

  <button @click="toggleStatus">Change</button>
  <div :class="[boldClass, greenClass]">Testing</div>
</template>

<script>
export default {
  data() {
    return {
      status: false,
      boldClass: 'bold',
      greenClass: 'success'
    }
  },
  methods: {
    toggleStatus() {
      this.status = !this.status
    }
  }
}
</script>

<style>
.success {
  color: green;
}
.failed {
  color: red;
}
.bold {
  font-weight: 700;
}
</style>