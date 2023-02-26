<script>
export default {
  data() {
    return {
      num1: 5,
      num2: 5
    }
  },
  methods: {
   showSum: function() {
    alert(this.num1 + this.num2);
   }
  }
}
</script>

<template>
  <div>{{ showSum() }}</div>
</template>

<style scoped></style>
