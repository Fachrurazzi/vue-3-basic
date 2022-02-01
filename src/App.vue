<template>
  <div>Ini adalah parent component</div>
  <child-component 
    v-for="name in names" 
    :text="name"
  />
</template>

<script>
import ChildComponent from './components/ChildComponent.vue'
export default {
  components:{ ChildComponent },
  data() {
    return {
      names: ['andi', 'anto', 'dono']
    }
  }
}
</script>

<style>

</style>