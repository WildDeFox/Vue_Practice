<script>
export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: "name1",
          surn: "surn1",
        },
        {
          id: 2,
          name: "name2",
          surn: "surn2",
        },
        {
          id: 3,
          name: "name3",
          surn: "surn3",
        },
      ],
      newItem: "",
    };
  },
  methods: {
    removeItem: function (id) {
      this.users = this.users.filter((user) => {
        return user.id !== id;
      })
    },
  },
};
</script>

<template>
  <ul>
   <li v-for="user in users" :key="user.id">
      {{ user.name }}
      {{ user.surn }}
      <button @click="removeItem(user.id)">remove</button>
  </li>
  </ul>
</template>
