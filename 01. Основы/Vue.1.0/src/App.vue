<script>
export default {
  data() {
    return {
     selected: 'Новосибирск',
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
  <select v-model="selected">
    <option>Москва</option>
    <option>Новосибирск</option>
    <option>Санкт-Петербург</option>
  </select>
  <p>{{ selected }}</p>
</template>