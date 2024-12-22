<script setup>
import {ref} from 'vue'
const color=ref('red')
const textSize=ref('43')
</script>

<template>
  <button class="text-white font-bold py-2 px-4 rounded" :class="[
    `bg-${color}-500`,
    `hover:bg-${color}-700`

  ]"
           :style=" `font-size: ${textSize}px`"
  >
    Button

  </button>
  <div class="mt-20">
    <input class="border border-gray-400 p-2" type="text" v-model="color" placeholder="color"/>
    <input class="border border-gray-400 p-2" type="text" v-model="textSize" placeholder="textSize"/>


  </div>

</template>

<style scoped>

</style>
