<template>
<div id="lifecycle">{{ message }}</div>

<button 
  @click="message= 'tulisan setelah dirender ulang'"
  >Update
</button>
</template>

<script>
export default {
  data() {
    return {
      message: 'first text'
    }
  },
  beforeCreate() {
    console.log('before create');
  },
  created() {
    console.log('created');
    console.log(this.message);
    console.log(document.getElementById('lifecycle'));
  },
  beforeMount() {
    console.log('before mount');
  },
  mounted() {
    console.log('mounted');
    console.log(this.message);
    console.log(document.getElementById('lifecycle'));
  },
  beforeUpdate() {
    console.log('before update');
    console.log(document.getElementById('lifecycle').textContent);
  },
  updated() {
    console.log('updated');
    console.log(document.getElementById('lifecycle').textContent);
  },
  beforeUnmount() {
    console.log('before unmount')
  },
  unmounted() {
    console.log('unmounted');
  }
}
</script>

<style>

</style>