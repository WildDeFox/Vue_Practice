<script>
export default {
  data() {
    
  },
  methods: {
    showTime: function() {
      let time = new Date;
      alert(time)
    }
  }
}
</script>

<template>
  <button @mouseover="showTime">Click me!</button>
</template>

<style scoped></style>
