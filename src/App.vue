<template>
<child>
  <template v-slot:default>
    <span>Ini adalah Judul</span>
  </template>

    <template v-slot:slotDua>
    <span>Ini adalah Kontent</span>
  </template>

    <template v-slot:slotTiga>
    <span>Ini adalah Footer</span>
  </template>
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