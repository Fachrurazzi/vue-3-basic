<template>
  <pre>{{ $data }}</pre>
  <button @click="onPress">Click Me</button>
</template>

<script>
import basicMixins from './mixins/basic'
import mergeMixins from './mixins/merge'
export default {
  mixins: [ basicMixins, mergeMixins ],
  data(){
    return {
      name: 'Fachrurazzi'
    }
  }
}
</script>