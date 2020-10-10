<template>
  <div id="app">
    {{count}}
    <button @click="add">增加</button>
  </div>
</template>

<script>
import {ref} from 'vue'
export default {
  name:'App',
  setup(){
    let count = ref(0)
    function add(){
      // console.log(count)
      count.value += 1
    }
    return { count,add }
  }
}
</script>

<style>
</style>
