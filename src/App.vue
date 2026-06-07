<script setup>
import { ref } from 'vue'
import ChildComp from './components/ChildComp.vue'

const childMsg = ref('No child msg yet')
// 発行されるイベントを宣言します
const emit = defineEmits(['response'])
</script>

<template>
  <ChildComp @response="(msg) => (childMsg = msg)" />
  <p>{{ childMsg }}</p>
</template>
