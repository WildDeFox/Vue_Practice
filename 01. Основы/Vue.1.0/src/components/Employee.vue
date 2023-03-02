<script>
  export default {
    props: ['name', 'surn', 'age', 'salary'],
    data() {
      return {
    
      }
    }
  }
</script>
<template>
  <p>{{ name }} {{ surn }} {{ age }} {{ salary }}</p>
</template>