<template>
  <div>Ini adalah parent component</div>
  <child-component/>
</template>

<script>
import ChildComponent from './components/ChildComponent.vue'
export default {
  components:{ ChildComponent }
}
</script>

<style>

</style>