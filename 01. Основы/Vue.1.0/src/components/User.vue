<script>
  export default {
    props: ['name', 'surn', 'args'],
    data() {
      return {
        
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
</template>