<script>
export default {
  data() {
    return {
     arr: [],
    };
  },
  methods: {
   show: function() {
    console.log(this.arr)
   }
  },
};
</script>

<template>
  <input type="checkbox" v-model="arr" value="v1">
  <input type="checkbox" v-model="arr" value="v2">
  <input type="checkbox" v-model="arr" value="v3">
  <button @click="show">Click me!</button>
</template>
