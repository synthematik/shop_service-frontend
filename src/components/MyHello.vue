<script setup>
  import {ref} from 'vue'

  let count = ref(0)

  function increament(){
    count.value++
  }

  function decreament(){
    count.value--
  }

  function updateCount(event){
    count.value = Number(event.target.value)
  }

</script>

<template>
  <p>{{ count }}</p>
  <button @click="increament">go</button>
  <button @click="decreament">go go</button>
  <input @input="updateCount"/>
  <input v-model="count"/>
</template>

<style scoped>

</style>