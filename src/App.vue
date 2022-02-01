<template>
  <div v-if="status">
    Ini Tampilkan
  </div>
  <button @click="toggleStatus">Toggle</button>

  <div v-if="status">True</div>
  <div v-else>False</div>
</template>

<script>
export default {
  data() {
    return {
      status: false
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

</style>