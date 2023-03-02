<script>
export default {
  data() {
    return {
     selected: 'Понедельник',
     options: ['Понедельник', "Вторник", "Среда", "Четверг", "Пятница", "Суббота", "Воскресенье"],
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
    <option v-for="option in options">{{ option }}</option>
  </select>
  <p>{{ selected }}</p>
</template>