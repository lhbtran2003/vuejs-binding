<script setup lang="ts">
import {computed, ref} from "vue";

const array = ref([])

const nameOfIndex = {
  football: "đá bóng",
  basketball: "bóng rổ",
  swimming: "bơi",
  study: "học"
}

const select = computed(() => {
  return array.value.map((hobby) => nameOfIndex[hobby])
})
</script>

<template>
  <div>
    đá bóng
    <input type="checkbox" value="football" v-model="array">
  </div>
  <div>
    bóng rổ
    <input type="checkbox" value="basketball" v-model="array">
  </div>
  <div>
    bơi
    <input type="checkbox" value="swimming" v-model="array">
  </div>
  <div>
    học
    <input type="checkbox" value="study" v-model="array">
  </div>

  <h3>
    Sở thích: {{select}}


  </h3>

</template>

<style scoped>

</style>