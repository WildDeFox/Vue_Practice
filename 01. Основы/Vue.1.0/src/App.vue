<script>
export default {
  data() {
    return {
      arr: ["item1", "item2", "item3", "item4"],
      newItem: '',
    };
  },
  methods: {
    addItem: function() {
      this.arr.push(this.newItem)
    },
    removeItem: function(index) {
      this.arr.splice(index, 1)
    }
  },
};
</script>

<template>
  <ul>
    <li v-for="(item, index) in arr" :key="index" @click="removeItem(index)">{{ item }}</li>
  </ul>
  <input type="text" v-model="newItem">
  <button @click="addItem">Добавить</button>
</template>
