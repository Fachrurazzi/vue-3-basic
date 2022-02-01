<template>
  <div v-once>{{ message }}</div>

  <button @click="message='hahahhihih'">Update</button>
</template>

<script>
export default {
  data() {
    return {
      message: 'Hi Guys'
    }
  }
}
</script>

<style>

</style>