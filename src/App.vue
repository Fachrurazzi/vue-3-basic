<template>
  <child ref="childComponent" @child-click="onPress"/>

  <button @click="clickSaya">Button dari Parent</button>
</template>

<script>
import Child from "./components/ChildComponent.vue"
export default {
  components: {Child},
  methods: {
    onPress(value) {
      console.log(value)
    },
    clickSaya() {
      this.$refs.childComponent.onClick();
    }
  }
}
</script>

<style>
</style>