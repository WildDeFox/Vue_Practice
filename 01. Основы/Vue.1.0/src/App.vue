<script>
export default {
  data() {
    return {
      visible1: false,
      visible2: true,
    }
  },
}
</script>

<template>
  <div v-if="visible1">Hello world!</div>
  <div v-if="visible2">How are you?</div>
</template>

