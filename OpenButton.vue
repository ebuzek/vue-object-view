<template>
  <button v-html="html" @click="$emit('click')"></button>
</template>

<script>
export default {
  name: 'openButton',
  props: [ 'html' ]
}
</script>

<style scoped>
  button {
    border: none;
    background: none;
  }
</style>
