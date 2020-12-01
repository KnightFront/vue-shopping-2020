<template>
  <div>
    <button @click="increment">+</button>
    <button @click="decrement">-</button>
    <p>{{num}}</p>
  </div>
</template>

<script>
  export default {
    props:["num"],
    data() {
      return {
        num:0
      }
    },
    methods: {
      increment(){
        this.num++
      },
      decrement(){
        this.num--
      }
    },
  }
</script>

<style>

</style>
