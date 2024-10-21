<script setup lang="ts">
import {ref} from "vue";

const value = ref('');
</script>

<template>
  <div>
    EMAIL:
    <input type="text" v-model="value">
  </div>
  <h3>Gía trị sau khi nhập: {{value}}</h3>
</template>

<style scoped>

</style>