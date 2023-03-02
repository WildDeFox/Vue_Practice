<script>
  import User from './components/User.vue';
  import Employee from './components/Employee.vue';

  export default {
    components: {
      User,
      Employee
    }
  }
</script>

<template>
  <User name="Nikita" surn="Kapurin" :args="['item1', 'item2', 'item3']"/>
  <Employee name="Jhon" surn="Smit" age="28"/>
</template>
