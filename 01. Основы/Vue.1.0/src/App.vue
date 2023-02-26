<script>
export default {
  data () {
    return {
      arr: [1, 2, 3],
      arr1: ['x', 'y', 'z']
    }
  }
}
</script>

<template>
  <p>{{ arr[0] + arr[1] + arr[2]}}</p>
  <p>{{ arr1[0] }}</p>
  <p>{{ arr1[1] }}</p>
  <p>{{ arr1[2] }}</p>
</template>

<style scoped></style>
