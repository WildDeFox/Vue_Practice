<script>
export default {
  data() {
    return {
      products: [
        {
          id: 1,
          name: "product1",
        },
        {
          id: 2,
          name: "product2",
        },
        {
          id: 3,
          name: "product3",
        },
      ],
      cssClasses: {
        red: false,
        active: true
      }
    };
  },
  methods: {
    click: function() {
      this.cssClasses.red = !this.cssClasses.red;
      this.cssClasses.active = !this.cssClasses.active;
    }
  }
};
</script>

<template>
  <ul>
    <li :class="cssClasses" v-for="elem in products" :key="elem.id">{{ elem.name }}</li>
  </ul>
  <button @click="click">Click</button>
</template>

<style>
.red {
  color: red
}

.active {
  color: yellow
}
</style>
