<template>
  <div>{{ message }}</div>

  <child 
    :model-value="message" 
    @update:model-value="message = $event"
    />

  <child v-model="message"/>
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