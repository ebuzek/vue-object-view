<template>
<span v-if="type === 'null'" class="object-tree-node-primitive object-tree-node-null">null</span>
<span v-else-if="type === 'undefined'" class="object-tree-node-primitive object-tree-node-undefined">undefined</span>
<span v-else-if="type === 'number'" class="object-tree-node-primitive object-tree-node-number">{{ value }}</span>
<span v-else-if="type === 'string'" class="object-tree-node-primitive object-tree-node-string">"{{ value }}"</span>
<span v-else-if="type === 'boolean'" class="object-tree-node-primitive object-tree-node-boolean">{{ value }}</span>
</template>

<script>
export default {
  name: 'objectTreeNodePrimitive',
  props: [ 'type', 'value' ]
}
</script>

<style scoped>
    .object-tree-node-null, .object-tree-node-undefined, .object-tree-node-boolean {
        font-weight: bold;
    }
</style>
