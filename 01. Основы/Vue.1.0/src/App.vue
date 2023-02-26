<script>
export default {
  data () {
    return {
      obj: {a: 1, b:2, c:3}
    }
  }
}
</script>

<template>
  <div>{{ obj['a'] + obj['b'] + obj['c'] }}</div>
</template>

<style scoped></style>
