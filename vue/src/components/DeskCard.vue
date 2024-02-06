<template>
<div id="app">
  <button @click="count++">
    Count is: {{ count }}
  </button>
</div>
</template>

<script>
import { createApp, ref } from 'vue'

createApp({
  setup() {
    return {
      count: ref(0)
    }
  }
}).mount('#app')
</script>

<style lang="scss" scoped>

</style>