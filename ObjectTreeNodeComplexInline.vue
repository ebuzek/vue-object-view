<template>
    <span>
    {
        <button v-if="!expanded" @click="expanded = true">...</button>
        <span v-if="expanded" v-for="key in Object.keys(this.value)"> {{ key }}: <objectTreeNode v-model="value[key]" :primary="false" />, </span>
    }
    </span>
</div>

</template>

<script>
import objectTreeNode from './ObjectTreeNode.vue';

export default {
  name: 'objectTreeNodeComplexInline',
  props: [ 'type', 'value', 'expanded' ],
  beforeCreate: function () {
    this.$options.components.objectTreeNode = require('./ObjectTreeNode.vue')
  },
  methods: {
    iterator() {
       
    }
  }
}
</script>

<style scoped>
    .object-tree-node-complex {
        padding-left: 10px;
    }
</style>
