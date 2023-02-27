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
      cssClasses: 'red active'
    };
  },
};
</script>

<template>
  <ul>
    <li :class="cssClasses" v-for="elem in products" :key="elem.id">{{ elem.name }}</li>
  </ul>
</template>

<style>
.red {
  color: red
}
</style>
