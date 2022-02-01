<template>
  <div>Ini adalah parent component</div>
  <child-component text="test123"/>
  <child-component :text="message"/>
</template>

<script>
import ChildComponent from './components/ChildComponent.vue'
export default {
  components:{ ChildComponent },
  data() {
    return {
      message: 'hallo world'
    }
  }
}
</script>

<style>

</style>