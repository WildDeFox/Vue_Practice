<script>
export default {
  data() {
    return {
      text: 'Hello world!',
      num1: 5,
      num2: 5
    }
  },
  methods: {
   change: function(newText) {
    this.text = newText;
   }
  }
}
</script>

<template>
  <div>{{ text }}</div>
  <button @click="change('How are you?')">Click Me!</button>
  <button @click="change('I am fine!')">Let`Go</button>
</template>

