<template>
  <satu />
</template>

<script>
import Satu from './components/ComponentSatu.vue'
export default {
  components: { Satu },
  data() {
    return {
      author: 'Fachrurazzi'
    }
  },
  provide() {
    return {
      providedAuthor: this.author
    }
  }
}
</script>

<style>
</style>