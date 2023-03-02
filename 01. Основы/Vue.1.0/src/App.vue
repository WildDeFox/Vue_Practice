<script>
  import User from './components/User.vue';
  import Employee from './components/Employee.vue';

  export default {
    data() {
      return {
        name: 'Jhon',
        surn: 'Smit',
        age: '25',
        salary: '80000'
      }
    },
    components: {
      User,
      Employee
    }
  }
</script>

<template>
  <User name="Nikita" surn="Kapurin" :args="['item1', 'item2', 'item3']"/>
  <Employee :name="name" :surn="surn" :age="age" :salary="salary"/>
</template>
