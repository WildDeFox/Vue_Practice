<script>
  export default {
    props: {
      name: String,
      surn: String, 
      age: Number,
      salary: Number
    },
    emits: ['remove'],
    data() {
      return {
    
      }
    },
  }
</script>
<template>
  <p>{{ name }} {{ surn }} {{ age }} {{ salary }}</p>
  <button @click="$emit('remove', id)">remove</button>
</template>