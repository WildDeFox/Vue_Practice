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
  <div>{{ showTime() }}</div>
</template>

<style scoped></style>
