<script setup>
import { ref } from 'vue'

const isActive = ref(false)
</script>

<template>
  <div>
    <button @click="isActive = !isActive">切换样式</button>
    <p :class="{ active: isActive }">这是一段动态样式的文字</p>
  </div>
</template>

<style>
.active {
  color: purple;
  font-weight: bold;
}
</style>
