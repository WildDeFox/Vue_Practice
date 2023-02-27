<script>
export default {
  data() {
    return {
      items: [1, 2, 3],
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
  <ul>
    <template v-for="elem in items">
      <li>{{ elem }}</li>
      <li class="divider"></li>
    </template>
  </ul>
</template>
