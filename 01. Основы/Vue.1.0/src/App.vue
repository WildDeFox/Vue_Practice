<script>
import User from "./components/User.vue";
import Employee from "./components/Employee.vue";

export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: "Jhon",
          surn: "Smit",
          age: "18",
          salary: "8000",
        },
        {
          id: 2,
          name: "Nikita",
          surn: "Kapurin",
          age: "25",
          salary: "100000",
        },
        {
          id: 3,
          name: "Rick",
          surn: "Sanchez",
          age: "45",
          salary: "80000",
        },
      ],
    };
  },
  components: {
    User,
    Employee,
  },
};
</script>

<template>
  <User name="Nikita" surn="Kapurin" :args="['item1', 'item2', 'item3']" />
  <Employee v-for="user in users"
  :name="user.name"
  :surn="user.surn"
  :age="user.age"
  :salary="user.salary"
  :key="user.id" />
</template>
