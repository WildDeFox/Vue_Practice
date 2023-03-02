<script>
export default {
  data() {
    return {
     isDisabled: true,
    };
  },
  methods: {
   click: function() {
    this.isDisabled = !this.isDisabled
   }
  },
};
</script>

<template>
  <input type="text" v-bind:disabled="isDisabled">
  <input type="checkbox" @click="click">Блокировать / Разблокировать
</template>