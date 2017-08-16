<template>
  <div class="vue-object-view">
    <objectTreeNode v-model="value" :primary="true" />
  </div>
</template>

<script>
import objectTreeNode from './ObjectTreeNode.vue';

export default {
  name: 'vueObjectView',
  props: [ 'value' ],
  components: {
      objectTreeNode
  }
}
</script>

<style scoped>
    div.vue-object-view {
        text-align: left;
        font-family: courier;
        overflow: hidden;
    }
</style>
