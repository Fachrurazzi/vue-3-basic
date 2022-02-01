<template>
<child>
  <template v-slot:default="{ data }">
    <span>Judul : {{ data }}</span>
  </template>

    <template v-slot:content="{ data }">
    <span>Konten : {{ data }}</span>
  </template>

    <template v-slot:footer="{ data }">
    <span>Footer : {{ data }} </span>
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