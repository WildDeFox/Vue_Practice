<script>
  export default {
    props: {
      name: String,
      surn: String, 
      age: Number,
      salary: Number
    },
    emits: ['showClick'],
    data() {
      return {
    
      }
    },
    methods: {
      handle () {
        this.$emit('showClick')
      }
    }
  }
</script>
<template>
  <p>{{ name }} {{ surn }} {{ age }} {{ salary }}</p>
  <button @click="handle">Show me click!</button>
</template>