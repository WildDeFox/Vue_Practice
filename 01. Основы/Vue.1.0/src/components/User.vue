<script>
  export default {
    props: ['name', 'surn', 'args'],
    emits: ['show'],
    data() {
      return {
        
      }
    },
    methods: {
      handle() {
        this.$emit('show')
      }
    }
  }
</script>
<template>
  {{ name }}
  {{ surn }}
  <ul>
    <li v-for="(arg, index) in args" :key="index">{{ arg }}</li>
  </ul>
  <button @click="handle">Click me</button>
</template>