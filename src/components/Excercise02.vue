<script setup lang="ts">
import {ref} from "vue";

const colour = ref('')
const dob = ref('')
const range = ref() // ko cần giá trị khởi tạo
const gender = ref(0);
</script>

<template>
  <div>
    nam
    <input type="radio" v-model="gender" name="gender" value="0">
  </div>

  <div>
    nữ
    <input type="radio" v-model="gender" name="gender" value="1">
  </div>
  <div>
    khác
    <input type="radio" v-model="gender" name="gender" value="2">
  </div>

  <h3 v-if="gender !== ''">
    Gioi tinh:
    <span v-if="gender == 0">Nam</span>
    <span v-else-if="gender == 1">Nữ</span>
    <span v-else="gender == 2">Khác</span>
  </h3>
</template>

<style scoped>

</style>