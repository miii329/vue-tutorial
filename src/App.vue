<script setup>
import { ref } from 'vue'

const count = ref(0)
function increment() {
  // コンポーネントの状態を更新する
  count.value++
}
</script>

<template>
  <!-- make this button work -->
  <button @click="increment">Count is: {{ count }}</button>
</template>
