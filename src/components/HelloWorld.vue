<script setup lang="ts">
import {ref, watch} from 'vue'
let count = ref(0);
let message = ref('');
watch(message, (newVal, oldVal) => {
  console.log("giá trị message: ", oldVal ,newVal)
})

</script>

<template>
  <input type="text"  v-model="message">
</template>

<style scoped>
</style>
