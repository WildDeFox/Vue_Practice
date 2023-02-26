<script>
export default {
  data() {
    return {
      num1: 5,
      num2: 5
    }
  },
  methods: {
   showSum: function(num) {
    alert(num * num);
   }
  }
}
</script>

<template>
  <button @click="showSum(2)">Click Me!</button>
  <button @click="showSum(3)">Let`Go</button>
</template>

<style scoped></style>
