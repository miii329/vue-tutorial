<script setup>
const emit = defineEmits(['response'])

// 引数つきで発行
emit('response', 'hello from child')
</script>

<template>
  <h2>Child component</h2>
</template>
