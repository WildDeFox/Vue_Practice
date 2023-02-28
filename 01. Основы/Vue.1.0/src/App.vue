<script>
export default {
  data() {
    return {
     choice: '',
    };
  },
  methods: {
   show: function() {
    console.log(this.choice)
   }
  },
};
</script>

<template>
  <input type="radio" name="radio" v-model="choice" value="v1">Русский 
  <input type="radio" name="radio" v-model="choice" value="v2">Французский
  <input type="radio" name="radio" v-model="choice" value="v3">Немецкий
  <button @click="show">Click me!</button>
</template>