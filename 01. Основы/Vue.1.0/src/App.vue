<script>
export default {
  data() {
    return {
      message: 'Hello'
    }
  }
  
};
</script>

<template>
  <input type="text" v-model="message">
  <p>{{ message }}</p>
</template>

<style>
</style>
