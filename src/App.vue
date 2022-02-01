<template>
  <child :message="'10'" :number="10" />
</template>

<script>
import Child from './components/ChildComponent.vue'
export default {
  components: { Child }
}
</script>

<style>
</style>