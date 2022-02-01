<template>
<child>
  <span>sisipan</span>
</child>

</template>

<script>
import Child from "./components/ChildComponent.vue"
export default {
  components: {Child},
  data() {
    return {
      message: ''
    }
  }
}
</script>

<style>
</style>