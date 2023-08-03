<script setup>
import { ref } from 'vue'

let home = ('')

const todolist = ref (['']) 

</script>

<template>
  <div class="input">
    <h2>To Do</h2>
    <input type="text"  v-model="home"
    placeholder="what todo">
    <button class="add" @click="todolist.push(home)">Add todo</button>
    <ol>
      <li v-for="items of todolist">{{'I want to:' + items }}</li>
    </ol>
  </div>


</template>

<style scoped>



</style>
