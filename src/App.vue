<template>
  <div>
    {{ message }}
  </div>

  <span :title="message">Balalalal</span>
</template>

<script>
export default {
  data() {
    return {
      message: 'Hi World'
    }
  }
}
</script>

<style>

</style>