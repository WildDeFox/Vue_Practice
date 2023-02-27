<script>
export default {
  data() {
    return {
      obj: {
        user1: "100$",
        user2: "200$",
        user3: "300$",
      },
    };
  },
  methods: {
    hide: function () {
      this.visible = !this.visible;
    },
  },
};
</script>

<template>
  <ul v-for="(elem, key, index) in obj">
    <li>{{ key }} - {{ elem }} - {{ index + 1 }}</li>
  </ul>
</template>
