<script>
  export default {
    props: {
      name: String,
      surn: String, 
      age: Number,
      salary: Number
    },
    data() {
      return {
    
      }
    }
  }
</script>
<template>
  <p>{{ name }} {{ surn }} {{ age }} {{ salary }}</p>
</template>